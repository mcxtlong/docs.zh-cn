---
title: 简化配置
ms.date: 03/30/2017
ms.assetid: dcbe1f84-437c-495f-9324-2bc09fd79ea9
ms.openlocfilehash: 13cf8bd46ef3aabb011cb2ddd207963235468662
ms.sourcegitcommit: 9b552addadfb57fab0b9e7852ed4f1f1b8a42f8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "61967890"
---
# <a name="simplified-configuration"></a>简化配置
配置 Windows Communication Foundation (WCF) 服务可能相当复杂的任务。 该任务涉及多个不同选项，并且有时会很难确定需要哪些设置。 虽然配置文件提高灵活性的 WCF 服务，它们也是带来了许多难以发现的问题。 [!INCLUDE[netfx_current_long](../../../includes/netfx-current-long-md.md)]解决了这些问题，并向用户提供了一种减小服务配置大小和降低复杂性的方法。  
  
## <a name="simplified-configuration"></a>简化配置  
 在 WCF 服务配置文件，<`system.serviceModel`> 部分包含 <`service`> 托管每个服务的元素。 <`service`> 元素包含一系列 <`endpoint`> 指定的每个服务和一组服务行为 （可选） 公开的终结点元素。 <`endpoint`> 元素指定地址、 绑定和协定公开终结点，也可以选择绑定配置和终结点行为。 <`system.serviceModel`> 部分还包含 <`behaviors`> 元素，它允许您指定服务或终结点行为。 下面的示例演示 <`system.serviceModel`> 配置文件的部分。  
  
```  
<system.serviceModel>  
  <behaviors>  
    <serviceBehaviors>  
      <behavior name="MyServiceBehavior">  
        <serviceMetadata httpGetEnabled="true">  
        <serviceDebug includeExceptionDetailInFaults="false">  
      </behavior>  
    </serviceBehaviors>  
  </behaviors>  
  <bindings>  
   <basicHttpBinding>  
      <binding name=MyBindingConfig"  
               maxBufferSize="100"  
               maxReceiveBufferSize="100" />  
   </basicHttpBinding>  
   </bindings>   <services>  
    <service behaviorConfiguration="MyServiceBehavior"  
             name="MyService">  
      <endpoint address=""  
                binding="basicHttpBinding"  
                contract="ICalculator"  
                bindingConfiguration="MyBindingConfig" />  
      <endpoint address="mex"  
                binding="mexHttpBinding"  
                contract="IMetadataExchange"/>  
    </service>  
  </services>  
</system.serviceModel>  
```  
  
 [!INCLUDE[netfx_current_short](../../../includes/netfx-current-short-md.md)] 可以通过删除的要求来配置 WCF 服务更加容易 <`service`> 元素。 如果未添加 <`service`> 部分，或添加任何终结点在 <`service`> 部分，并且你的服务未以编程方式定义任何终结点，则一组默认终结点会自动添加到你的服务，每个服务基址和服务实现的每个协定。 在上述每个终结点中，终结点地址与基址相对应，绑定由基址方案确定，协定即为服务实现的协定。 如果你不需要指定任何终结点或服务行为，或者不需要更改任何绑定设置，则完全不必指定服务配置文件。 如果服务实现了两个协定，并且主机同时启用了 HTTP 和 TCP 传输，服务主机将创建四个默认终结点，使用每个传输的每一协定各对应一个终结点。 若要创建默认终结点，服务主机必须了解要使用的绑定。 这些设置指定在 <`protocolMappings`> 节中 <`system.serviceModel`> 部分。 <`protocolMappings`> 部分包含映射到绑定类型的传输协议方案的列表。 服务主机使用传递到它的基址来确定要使用的绑定。 下面的示例使用 <`protocolMappings`> 元素。  
  
> [!WARNING]
>  更改默认配置元素（如绑定或行为）可能会影响在配置层次结构的较低级别中定义的服务，因为这些服务可能使用这些默认绑定和行为。 因而，更改默认绑定和行为的任何人员都需要注意，这些更改可能会影响层次结构中的其他服务。  
  
> [!NOTE]
>  承载于 Internet 信息服务 (IIS) 或 Windows 进程激活服务 (WAS) 下的服务使用虚拟目录作为其基址。  
  
```xml  
<protocolMapping>  
  <add scheme="http"     binding="basicHttpBinding" bindingConfiguration="MyBindingConfiguration"/>  
  <add scheme="net.tcp"  binding="netTcpBinding"/>  
  <add scheme="net.pipe" binding="netNamedPipeBinding"/>  
  <add scheme="net.msmq" binding="netMSMQBinding"/>  
</protocolMapping>  
```  
  
 在上一示例中，基址以“http”方案开头的终结点使用 <xref:System.ServiceModel.BasicHttpBinding>。 基址以“net.tcp”方案开头的终结点使用 <xref:System.ServiceModel.NetTcpBinding>。 你可以在本地 App.config 或 Web.config 文件中重写相应设置。  
  
 中的每个元素 <`protocolMappings`> 部分必须指定方案和绑定。 或者可以指定`bindingConfiguration`绑定中指定配置的属性 <`bindings`> 配置文件的部分。 如果未指定 `bindingConfiguration`，则使用相应绑定类型的匿名绑定配置。  
  
 为默认终结点配置服务行为，应使用匿名 <`behavior`> 部分中 <`serviceBehaviors`> 部分。 任何未命名 <`behavior`> 中的元素 <`serviceBehaviors`> 用于配置服务行为。 例如，下面的配置文件对主机中的所有服务启用服务元数据发布。  
  
```xml  
<system.serviceModel>  
    <behaviors>  
      <serviceBehaviors>  
        <behavior>  
          <serviceMetadata httpGetEnabled="True"/>  
        </behavior>  
      </serviceBehaviors>  
    </behaviors>    <!-- No <service> tag is necessary. Default endpoints are added to the service -->  
    <!-- The service behavior with name="" is picked up by the service -->  
 </system.serviceModel>  
```  
  
 终结点行为配置通过使用匿名 <`behavior`> 部分中 <`serviceBehaviors`> 部分。  
  
 下面示例中的配置文件使用简化配置模型，它等效于本主题开头的配置文件。  
  
```xml  
<system.serviceModel>
    <behaviors>
      <serviceBehaviors>
        <behavior>
          <serviceMetadata httpGetEnabled="true" />
          <serviceDebug includeExceptionDetailInFaults="false" />
        </behavior>
      </serviceBehaviors>
    </behaviors>
    <bindings>
       <basicHttpBinding>
          <binding maxBufferSize="100"
                   maxReceiveBufferSize="100" />
       </basicHttpBinding>
    </bindings>
    <!-- No <service> tag is necessary. Default endpoints will be added to the service -->
    <!-- The service behavior with name="" will be picked up by the service -->
    <protocolMapping>
      <add scheme="http" binding="basicHttpBinding" />
  </protocolMapping>
  </system.serviceModel>
```  
  
> [!IMPORTANT]
>  此功能只与 WCF 服务配置相关，与客户端配置无关。 大多数时候，使用 svcutil.exe 之类的工具或从 Visual Studio 添加服务引用将生成 WCF 客户端配置。 如果您在手动配置 WCF 客户端将需要添加\<客户端 > 配置元素，并指定你想要调用任何终结点。  
  
## <a name="see-also"></a>请参阅

- [使用配置文件配置服务](../../../docs/framework/wcf/configuring-services-using-configuration-files.md)
- [配置服务绑定](../../../docs/framework/wcf/configuring-bindings-for-wcf-services.md)
- [配置系统提供的绑定](../../../docs/framework/wcf/feature-details/configuring-system-provided-bindings.md)
- [配置服务](../../../docs/framework/wcf/configuring-services.md)
- [配置 WCF 服务](configuring-services.md)
- [在代码中配置 WCF 服务](../../../docs/framework/wcf/configuring-wcf-services-in-code.md)
