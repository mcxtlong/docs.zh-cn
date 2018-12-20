# <a name="contributing"></a><span data-ttu-id="25743-101">参与</span><span class="sxs-lookup"><span data-stu-id="25743-101">Contributing</span></span>

<span data-ttu-id="25743-102">感谢你对参与 .NET 文档的关注！</span><span class="sxs-lookup"><span data-stu-id="25743-102">Thank you for your interest in contributing to the .NET documentation!</span></span>

> <span data-ttu-id="25743-103">我们正在将我们的指导原则转变为网站级参与指南。</span><span class="sxs-lookup"><span data-stu-id="25743-103">We're in the process of moving our guidelines into a site-wide contribution guide.</span></span> 
> <span data-ttu-id="25743-104">若要查看新指南，请访问 [Microsoft Docs 参与者指南概述](https://docs.microsoft.com/contribute/)。</span><span class="sxs-lookup"><span data-stu-id="25743-104">To see the new guidance, visit [Microsoft Docs contributor guide overview](https://docs.microsoft.com/contribute/).</span></span>

<span data-ttu-id="25743-105">本文档介绍了参与到 [.NET 文档站点](https://docs.microsoft.com/dotnet)上托管的文章和代码示例中的过程。</span><span class="sxs-lookup"><span data-stu-id="25743-105">The document covers the process for contributing to the articles and code samples that are hosted on the [.NET documentation site](https://docs.microsoft.com/dotnet).</span></span> <span data-ttu-id="25743-106">参与内容可简（更正拼写错误），可繁（编写新文章）。</span><span class="sxs-lookup"><span data-stu-id="25743-106">Contributions may be as simple as typo corrections or as complex as new articles.</span></span>

* [<span data-ttu-id="25743-107">参与流程</span><span class="sxs-lookup"><span data-stu-id="25743-107">Process for contributing</span></span>](#process-for-contributing)
* [<span data-ttu-id="25743-108">C# 交互式体验</span><span class="sxs-lookup"><span data-stu-id="25743-108">The C# interactive experience</span></span>](#the-c-interactive-experience)
* [<span data-ttu-id="25743-109">注意事项</span><span class="sxs-lookup"><span data-stu-id="25743-109">DOs and DON'Ts</span></span>](#dos-and-donts)
* [<span data-ttu-id="25743-110">参与者许可协议</span><span class="sxs-lookup"><span data-stu-id="25743-110">Contributor License Agreement</span></span>](#contributor-license-agreement)

<span data-ttu-id="25743-111">此存储库包含适用于 .NET 的概念文档。</span><span class="sxs-lookup"><span data-stu-id="25743-111">This repository contains the conceptual documentation for .NET.</span></span> <span data-ttu-id="25743-112">.NET 文档站点建立在多个存储库的基础上，还包括下面这个：</span><span class="sxs-lookup"><span data-stu-id="25743-112">The .NET documentation site is built from multiple repositories in addition to this one:</span></span>

- [<span data-ttu-id="25743-113">代码示例和代码片段</span><span class="sxs-lookup"><span data-stu-id="25743-113">Code samples and snippets</span></span>](https://github.com/dotnet/samples)
- [<span data-ttu-id="25743-114">API 参考</span><span class="sxs-lookup"><span data-stu-id="25743-114">API reference</span></span>](https://github.com/dotnet/dotnet-api-docs)
- [<span data-ttu-id="25743-115">.NET Compiler Platform SDK 参考</span><span class="sxs-lookup"><span data-stu-id="25743-115">.NET Compiler Platform SDK reference</span></span>](https://github.com/dotnet/roslyn-api-docs)

<span data-ttu-id="25743-116">可在此处跟踪所有这些存储库的问题和任务。</span><span class="sxs-lookup"><span data-stu-id="25743-116">Issues and tasks for all these repositories are tracked here.</span></span>

## <a name="process-for-contributing"></a><span data-ttu-id="25743-117">参与流程</span><span class="sxs-lookup"><span data-stu-id="25743-117">Process for contributing</span></span>

<span data-ttu-id="25743-118">需要对 [Git 和 GitHub.com](https://guides.github.com/activities/hello-world/) 有基本的理解。</span><span class="sxs-lookup"><span data-stu-id="25743-118">You need a basic understanding of [Git and GitHub.com](https://guides.github.com/activities/hello-world/).</span></span>

<span data-ttu-id="25743-119">**步骤 1：** 对于小更改，可跳过这一步。</span><span class="sxs-lookup"><span data-stu-id="25743-119">**Step 1:** Skip this step for small changes.</span></span> <span data-ttu-id="25743-120">如果有意编写新内容或彻底修改现有内容，请打开[问题](https://github.com/dotnet/docs/issues)，描述要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="25743-120">If you're interested in writing new content or in thoroughly revising existing content, open an [issue](https://github.com/dotnet/docs/issues) describing what you want to do.</span></span>
<span data-ttu-id="25743-121">“文档”文件夹中的内容划分为在目录 (TOC) 中反应的不同部分。</span><span class="sxs-lookup"><span data-stu-id="25743-121">The content inside the **docs** folder is organized into sections that are reflected in the Table of Contents (TOC).</span></span> <span data-ttu-id="25743-122">定义主题在 TOC 中的位置。</span><span class="sxs-lookup"><span data-stu-id="25743-122">Define where the topic will be located in the TOC.</span></span> <span data-ttu-id="25743-123">获取对建议的反馈。</span><span class="sxs-lookup"><span data-stu-id="25743-123">Get feedback on your proposal.</span></span>

<span data-ttu-id="25743-124">或</span><span class="sxs-lookup"><span data-stu-id="25743-124">-or-</span></span>

<span data-ttu-id="25743-125">还可以从现有问题中进行选择，了解哪些是热门的社区发布内容。</span><span class="sxs-lookup"><span data-stu-id="25743-125">You can also choose from existing issues for which community contributions are welcome.</span></span> <span data-ttu-id="25743-126">[.NET 社区参与者项目](https://github.com/dotnet/docs/projects/35)列出了许多可用于社区参与者的工作项。</span><span class="sxs-lookup"><span data-stu-id="25743-126">[Projects for .NET Community contributors](https://github.com/dotnet/docs/projects/35) lists many of the work items that are available for community contributors.</span></span> <span data-ttu-id="25743-127">根据你的兴趣和承诺水平，可从以下类别的问题中作出选择：</span><span class="sxs-lookup"><span data-stu-id="25743-127">Depending on your interests and level of commitment, you can choose from issues in the following categories:</span></span>

- <span data-ttu-id="25743-128">**维护**。</span><span class="sxs-lookup"><span data-stu-id="25743-128">**Maintenance**.</span></span> <span data-ttu-id="25743-129">此类别包括相当简单的发布内容，如修复损坏或不正确的链接，添加缺少的代码示例，或处理有限内容问题。</span><span class="sxs-lookup"><span data-stu-id="25743-129">This category includes fairly simple contributions, such as fixing broken or incorrect links, adding missing code examples, or addressing limited content issues.</span></span> <span data-ttu-id="25743-130">在某些情况下，这些问题可能会涉及大量文件。</span><span class="sxs-lookup"><span data-stu-id="25743-130">In some cases, these issues may concern large numbers of files.</span></span> <span data-ttu-id="25743-131">在此情况下，应让我们知道在开始之前你想要处理的内容。</span><span class="sxs-lookup"><span data-stu-id="25743-131">In that case, you should let us know what you'd like to work on before you begin.</span></span>

- <span data-ttu-id="25743-132">**内容更新**。</span><span class="sxs-lookup"><span data-stu-id="25743-132">**Content updates**.</span></span> <span data-ttu-id="25743-133">考虑到文档集比较庞大，内容很容易过时且需要修改。</span><span class="sxs-lookup"><span data-stu-id="25743-133">Given the enormity of the doc set, content easily becomes outdated and requires revision.</span></span> <span data-ttu-id="25743-134">此外，由于各种原因，会对一些内容进行备份甚至双重备份。</span><span class="sxs-lookup"><span data-stu-id="25743-134">In addition, for a variety of reason, some content has been duplicated or even triplicated.</span></span> <span data-ttu-id="25743-135">更新内容包括确保单个主题是最新的，或者修改功能区域中的内容以消除重复，并确保所有唯一内容都保存在较小的文档集中。</span><span class="sxs-lookup"><span data-stu-id="25743-135">Updating content involves making sure that individual topics are current or revising content in a feature area to eliminate duplication and ensure that all unique content is preserved in the smaller documentation set.</span></span>

- <span data-ttu-id="25743-136">**新内容创作**。</span><span class="sxs-lookup"><span data-stu-id="25743-136">**New content authoring**.</span></span> <span data-ttu-id="25743-137">如果了解如何创作你自己的主题，这些问题将列出我们知道要添加到文档集的主题。</span><span class="sxs-lookup"><span data-stu-id="25743-137">If you're interested in authoring your own topic, these issues list topics that we know we'd like to add to our doc set.</span></span> <span data-ttu-id="25743-138">不过，在你开始研究某个主题之前，请告知我们。</span><span class="sxs-lookup"><span data-stu-id="25743-138">Let us know before you begin working on a topic, though.</span></span> <span data-ttu-id="25743-139">如果你有意编写此处未列出的主题，请提问。</span><span class="sxs-lookup"><span data-stu-id="25743-139">If you're interested in writing a topic that isn't listed here, open an issue.</span></span> 

<span data-ttu-id="25743-140">此外可以查看我们的[待解决问题](https://github.com/dotnet/docs/issues)列表，并自愿参与你感兴趣的工作。</span><span class="sxs-lookup"><span data-stu-id="25743-140">You can also look at our [open issues](https://github.com/dotnet/docs/issues) list and volunteer to work on the ones you're interested in.</span></span> <span data-ttu-id="25743-141">我们使用[空缺](https://github.com/dotnet/docs/labels/up-for-grabs)标签来标记公开供参与的问题。</span><span class="sxs-lookup"><span data-stu-id="25743-141">We use the [up-for-grabs](https://github.com/dotnet/docs/labels/up-for-grabs) label to tag issues open for contribution.</span></span> 

<span data-ttu-id="25743-142">**步骤 2：** 根据需要派生 `/dotnet/docs`、`dotnet/samples` 或 `dotnet/dotnet-api-docs` 存储库分支，并为更改创建一个分支。</span><span class="sxs-lookup"><span data-stu-id="25743-142">**Step 2:** Fork the `/dotnet/docs`, `dotnet/samples` or `dotnet/dotnet-api-docs` repos as needed and create a branch for your changes.</span></span>

<span data-ttu-id="25743-143">对于较小的更改，可以使用 GitHub 的 Web 界面。</span><span class="sxs-lookup"><span data-stu-id="25743-143">For small changes, you can use GitHub's web interface.</span></span> <span data-ttu-id="25743-144">只需单击要更改的文件上的“编辑此项目分支中的文件”。</span><span class="sxs-lookup"><span data-stu-id="25743-144">Simply click the **Edit the file in your fork of this project** on the file you'd like to change.</span></span> <span data-ttu-id="25743-145">在提交所做的更改时，GitHub 会为你创建新分支。</span><span class="sxs-lookup"><span data-stu-id="25743-145">GitHub creates the new branch for you when you submit the changes.</span></span>

<span data-ttu-id="25743-146">**步骤 3：** 对该新分支进行更改。</span><span class="sxs-lookup"><span data-stu-id="25743-146">**Step 3:** Make the changes on this new branch.</span></span>

<span data-ttu-id="25743-147">如果要新建主题，可以使用此[模板文件](./styleguide/template.md)作为起点。</span><span class="sxs-lookup"><span data-stu-id="25743-147">If it's a new topic, you can use this [template file](./styleguide/template.md) as your starting point.</span></span> <span data-ttu-id="25743-148">它包含编写指南，还介绍了每篇文章所需的元数据，例如作者信息。</span><span class="sxs-lookup"><span data-stu-id="25743-148">It contains the writing guidelines and also explains the metadata required for each article, such as author information.</span></span>

<span data-ttu-id="25743-149">导航到与步骤 1 中为文章确定的 TOC 位置对应的文件夹。</span><span class="sxs-lookup"><span data-stu-id="25743-149">Navigate to the folder that corresponds to the TOC location determined for your article in step 1.</span></span>
<span data-ttu-id="25743-150">该文件夹包含该部分中的所有文章的 Markdown 文件。</span><span class="sxs-lookup"><span data-stu-id="25743-150">That folder contains the Markdown files for all articles in that section.</span></span>
<span data-ttu-id="25743-151">如有必要，可以创建一个新文件夹来放置内容文件。</span><span class="sxs-lookup"><span data-stu-id="25743-151">If necessary, create a new folder to place the files for your content.</span></span> <span data-ttu-id="25743-152">该部分的主要文章称为“index.md”。</span><span class="sxs-lookup"><span data-stu-id="25743-152">The main article for that section is called *index.md*.</span></span>
<span data-ttu-id="25743-153">对于图像和其他静态资源，在包含项目的文件夹内创建名为“媒体”的子文件夹（如果尚不存在）。</span><span class="sxs-lookup"><span data-stu-id="25743-153">For images and other static resources, create a subfolder called **media** inside the folder that contains your article, if it doesn't already exist.</span></span> <span data-ttu-id="25743-154">在“媒体”文件夹中，使用项目名称创建一个子文件夹（索引文件除外）。</span><span class="sxs-lookup"><span data-stu-id="25743-154">Inside the **media** folder, create a subfolder with the article name (except for the index file).</span></span>
<span data-ttu-id="25743-155">在存储库根目录下的“示例”文件夹中包含更大示例。</span><span class="sxs-lookup"><span data-stu-id="25743-155">Include larger samples in the *samples* folder under the root of the repo.</span></span>

<span data-ttu-id="25743-156">请务必遵循正确的 Markdown 语法。</span><span class="sxs-lookup"><span data-stu-id="25743-156">Be sure to follow the proper Markdown syntax.</span></span> <span data-ttu-id="25743-157">有关详细信息，请参阅[风格指南](./styleguide/template.md)。</span><span class="sxs-lookup"><span data-stu-id="25743-157">For more information, see the [style guide](./styleguide/template.md).</span></span>

### <a name="example-structure"></a><span data-ttu-id="25743-158">结构示例</span><span class="sxs-lookup"><span data-stu-id="25743-158">Example structure</span></span>

    docs
      /about
      /core
        /porting
          porting-overview.md
          /media
            /porting-overview
                portability_report.png

<span data-ttu-id="25743-159">**步骤 4：** 将拉取请求 (PR) 从分支提交到 `dotnet/docs/master`。</span><span class="sxs-lookup"><span data-stu-id="25743-159">**Step 4:** Submit a Pull Request (PR) from your branch to `dotnet/docs/master`.</span></span>

<span data-ttu-id="25743-160">每个 PR 通常应该一次解决一个问题。</span><span class="sxs-lookup"><span data-stu-id="25743-160">Each PR should usually address one issue at a time.</span></span> <span data-ttu-id="25743-161">PR 可以修改一个或多个文件。</span><span class="sxs-lookup"><span data-stu-id="25743-161">The PR can modify one or multiple files.</span></span> <span data-ttu-id="25743-162">如果要处理不同文件的多个修补程序，最好是使用单独的 PR。</span><span class="sxs-lookup"><span data-stu-id="25743-162">If you're addressing multiple fixes on different files, separate PRs are preferred.</span></span>

<span data-ttu-id="25743-163">如果 PR 正在解决现有问题，请将 `Fixes #Issue_Number` 关键字添加到提交消息或 PR 描述中。</span><span class="sxs-lookup"><span data-stu-id="25743-163">If your PR is addressing an existing issue, add the `Fixes #Issue_Number` keyword to the commit message or PR description.</span></span> <span data-ttu-id="25743-164">以此，在合并 PR 时将自动关闭该问题。</span><span class="sxs-lookup"><span data-stu-id="25743-164">That way, the issue is automatically closed when the PR is merged.</span></span> <span data-ttu-id="25743-165">有关详细信息，请参阅[通过提交消息关闭问题](https://help.github.com/articles/closing-issues-via-commit-messages/)。</span><span class="sxs-lookup"><span data-stu-id="25743-165">For more information, see [Closing issues via commit messages](https://help.github.com/articles/closing-issues-via-commit-messages/).</span></span>

<span data-ttu-id="25743-166">.NET 团队将审核 PR，并告知是否需要进行任何其他更新/更改才能批准。</span><span class="sxs-lookup"><span data-stu-id="25743-166">The .NET team will review your PR and let you know if there are any other updates/changes necessary in order to approve it.</span></span>

<span data-ttu-id="25743-167">**步骤 5：** 与团队讨论后，对分支进行必要的更新。</span><span class="sxs-lookup"><span data-stu-id="25743-167">**Step 5:** Make any necessary updates to your branch as discussed with the team.</span></span>

<span data-ttu-id="25743-168">一旦应用反馈并批准所做的更改，维护人员会将 PR 合并到主分支。</span><span class="sxs-lookup"><span data-stu-id="25743-168">The maintainers will merge your PR into the master branch once feedback has been applied and your change is approved.</span></span>

<span data-ttu-id="25743-169">我们会以某种节奏，将所有提交从主分支推送到实时分支，你将能在 https://docs.microsoft.com/dotnet/ 中实时看到你的参与内容。</span><span class="sxs-lookup"><span data-stu-id="25743-169">On a certain cadence, we push all commits from master branch into the live branch and then you'll be able to see your contribution live at https://docs.microsoft.com/dotnet/.</span></span>

### <a name="contributing-to-samples"></a><span data-ttu-id="25743-170">提供示例</span><span class="sxs-lookup"><span data-stu-id="25743-170">Contributing to samples</span></span>

<span data-ttu-id="25743-171">我们对存储库中存在的代码做如下区分：</span><span class="sxs-lookup"><span data-stu-id="25743-171">We make the following distinction for code that exists in our repository:</span></span>

- <span data-ttu-id="25743-172">示例：读者可以下载并运行示例。</span><span class="sxs-lookup"><span data-stu-id="25743-172">Samples: readers can download and run the samples.</span></span> <span data-ttu-id="25743-173">所有示例应都为完整的应用程序或库。</span><span class="sxs-lookup"><span data-stu-id="25743-173">All samples should be complete applications or libraries.</span></span> <span data-ttu-id="25743-174">在示例创建库的位置，它应包括单元测试或允许读者运行代码的应用程序。</span><span class="sxs-lookup"><span data-stu-id="25743-174">Where the sample creates a library, it should include unit tests or an application that lets readers run the code.</span></span>

- <span data-ttu-id="25743-175">代码段：说明较小的概念或任务。</span><span class="sxs-lookup"><span data-stu-id="25743-175">Snippets: illustrate a smaller concept or task.</span></span> <span data-ttu-id="25743-176">它们可以编译，但并不是完整的应用程序。</span><span class="sxs-lookup"><span data-stu-id="25743-176">They compile but they are not intended to be complete applications.</span></span>

<span data-ttu-id="25743-177">所有代码都位于 [dotnet/samples](https://github.com/dotnet/samples) 存储库中。</span><span class="sxs-lookup"><span data-stu-id="25743-177">Code all lives in the [dotnet/samples](https://github.com/dotnet/samples) repository.</span></span> <span data-ttu-id="25743-178">我们正在努力建立一个示例文件夹结构与文档文件夹结构匹配的模型。</span><span class="sxs-lookup"><span data-stu-id="25743-178">We are working toward a model where our samples folder structure matches our docs folder structure.</span></span> <span data-ttu-id="25743-179">我们将遵循如下标准：</span><span class="sxs-lookup"><span data-stu-id="25743-179">Standards that we follow are:</span></span>

- <span data-ttu-id="25743-180">顶级“代码段”文件夹包含小型、集中式示例代码段。</span><span class="sxs-lookup"><span data-stu-id="25743-180">The top level *snippets* folder contains snippets for small, focused samples.</span></span>
- <span data-ttu-id="25743-181">API 参考示例已置于遵循以下模式的文件夹中：代码段/\<语言>/api/\<命名空间>/\<apiname>。</span><span class="sxs-lookup"><span data-stu-id="25743-181">API reference samples have been in a folder following this pattern: *snippets/\<language>/api/\<namespace>/\<apiname>*.</span></span>
- <span data-ttu-id="25743-182">其他顶级文件夹与“文档”存储库中的顶级文件夹匹配。</span><span class="sxs-lookup"><span data-stu-id="25743-182">Other top-level folders match the top level folders in the *docs* repository.</span></span> <span data-ttu-id="25743-183">例如，文档存储库具有“机器学习/教程”文件夹，机器学习教程示例位于“示例/机器学习/教程”文件夹。</span><span class="sxs-lookup"><span data-stu-id="25743-183">For example, the docs repository has a *machine-learning/tutorials* folder, and the samples for machine learning tutorials are in the *samples/machine-learning/tutorials* folder.</span></span>

<span data-ttu-id="25743-184">此外，“核心”和“标准”文件夹下的所有示例都应在 .NET Core 支持的所有平台上构建和运行。</span><span class="sxs-lookup"><span data-stu-id="25743-184">In addition, all samples under the *core* and *standard* folders should build and run on all platforms supported by .NET Core.</span></span> <span data-ttu-id="25743-185">我们的 CI 生成系统会强制此要求。</span><span class="sxs-lookup"><span data-stu-id="25743-185">Our CI build system will enforce that.</span></span> <span data-ttu-id="25743-186">顶级“框架”文件夹包含仅在 Windows 上生成和验证的示例。</span><span class="sxs-lookup"><span data-stu-id="25743-186">The top level *framework* folder contains samples that are only built and validated on Windows.</span></span>

<span data-ttu-id="25743-187">我们可以在文档存储库添加新内容时扩展这些目录。</span><span class="sxs-lookup"><span data-stu-id="25743-187">We may expand these directories as the docs repository adds new content.</span></span> <span data-ttu-id="25743-188">例如，我们将添加 Xamarin 目录，如 `xamarin-ios` 和 `xamarin-android` 目录。</span><span class="sxs-lookup"><span data-stu-id="25743-188">For example, we will add Xamarin directories, like `xamarin-ios` and `xamarin-android` directories.</span></span>

<span data-ttu-id="25743-189">创建的每个完整示例都应包含“readme.md”文件。</span><span class="sxs-lookup"><span data-stu-id="25743-189">Each complete sample that you create should contain a *readme.md* file.</span></span> <span data-ttu-id="25743-190">此文件应包含示例的简短说明（一个或两个段落）。</span><span class="sxs-lookup"><span data-stu-id="25743-190">This file should contain a short description of the sample (one or two paragraphs).</span></span> <span data-ttu-id="25743-191">“readme.md”应告知读者通过研究此示例他们将了解到的内容。</span><span class="sxs-lookup"><span data-stu-id="25743-191">Your *readme.md* should tell readers what they will learn by exploring this sample.</span></span> <span data-ttu-id="25743-192">“Readme.md”文件还应包含到 [.NET 文档站点](https://docs.microsoft.com/dotnet/welcome)上实时文档的链接。</span><span class="sxs-lookup"><span data-stu-id="25743-192">The *readme.md* file should also contain a link to the live document on the [.NET documentation site](https://docs.microsoft.com/dotnet/welcome).</span></span>
<span data-ttu-id="25743-193">要确定存储库中给定文件映射到该站点的位置，请将存储库路径中的 `/docs` 替换为 `http://docs.microsoft.com/dotnet/articles`。</span><span class="sxs-lookup"><span data-stu-id="25743-193">To determine where a given file in the repository maps to that site, replace `/docs` in the repository path with `http://docs.microsoft.com/dotnet/articles`.</span></span>

<span data-ttu-id="25743-194">主题还将包含该示例的链接。</span><span class="sxs-lookup"><span data-stu-id="25743-194">Your topic will also contain links to the sample.</span></span> <span data-ttu-id="25743-195">直接链接到 GitHub 上的示例文件夹。</span><span class="sxs-lookup"><span data-stu-id="25743-195">Link directly to the sample's folder on GitHub.</span></span>

<span data-ttu-id="25743-196">有关详细信息，请参阅[示例自述文件](https://github.com/dotnet/samples/blob/master/README.md)。</span><span class="sxs-lookup"><span data-stu-id="25743-196">For more information, see the [Samples Readme](https://github.com/dotnet/samples/blob/master/README.md).</span></span>

## <a name="the-c-interactive-experience"></a><span data-ttu-id="25743-197">C# 交互式体验</span><span class="sxs-lookup"><span data-stu-id="25743-197">The C# interactive experience</span></span> #

<span data-ttu-id="25743-198">C# 中的简短代码示例可以使用 `csharp-interactive` 语言标记来指定浏览器中运行的 C# 示例。</span><span class="sxs-lookup"><span data-stu-id="25743-198">Short code samples in C# can use the `csharp-interactive` language tag to specify a C# sample that runs in the browser.</span></span> <span data-ttu-id="25743-199">（内联代码示例使用 `csharp-interactive` 标记，对于源代码中包含的代码段，请使用 `code-csharp-interactive` 标记。）这些代码示例在本文中显示一个代码窗口和一个输出窗口。</span><span class="sxs-lookup"><span data-stu-id="25743-199">(Inline code samples use the `csharp-interactive` tag, for snippets included from source, use the `code-csharp-interactive` tag.) These code samples display a code window and an output window in the article.</span></span> <span data-ttu-id="25743-200">输出窗口显示用户运行示例后执行交互式代码的任何输出。</span><span class="sxs-lookup"><span data-stu-id="25743-200">The output window displays any output from executing the interactive code once the user has run the sample.</span></span> 

<span data-ttu-id="25743-201">C# 交互式体验改变了我们使用示例的方式。</span><span class="sxs-lookup"><span data-stu-id="25743-201">The C# interactive experience changes how we work with samples.</span></span> <span data-ttu-id="25743-202">访问者可以运行该示例以查看结果。</span><span class="sxs-lookup"><span data-stu-id="25743-202">Visitors can run the sample to see the results.</span></span> <span data-ttu-id="25743-203">很多因素有助于确定示例或相应的文本是否应包括有关输出的信息。</span><span class="sxs-lookup"><span data-stu-id="25743-203">A number of factors help determine if the sample or corresponding text should include information about the output.</span></span>

### <a name="when-to-display-the-expected-output-without-running-the-sample"></a><span data-ttu-id="25743-204">在不运行示例的情况下何时显示预期输出</span><span class="sxs-lookup"><span data-stu-id="25743-204">When to display the expected output without running the sample</span></span>

- <span data-ttu-id="25743-205">面向初学者的文章应提供输出，以便读者能够将其工作输出与预期答案进行比较。</span><span class="sxs-lookup"><span data-stu-id="25743-205">Articles intended for beginners should provide output so that readers can compare the output of their work with the expected answer.</span></span>
- <span data-ttu-id="25743-206">输出对于主题不可或缺的示例应显示该输出。</span><span class="sxs-lookup"><span data-stu-id="25743-206">Samples where the output is integral to the topic should display that output.</span></span> <span data-ttu-id="25743-207">例如，关于格式化文本的文章应在不运行示例的情况下显示文本格式。</span><span class="sxs-lookup"><span data-stu-id="25743-207">For example, articles on formatted text should show the text format without running the sample.</span></span>
- <span data-ttu-id="25743-208">当示例和预期输出都很短时，请考虑显示输出。</span><span class="sxs-lookup"><span data-stu-id="25743-208">When both the sample and the expected output is short, consider showing the output.</span></span> <span data-ttu-id="25743-209">它可以节省一些时间。</span><span class="sxs-lookup"><span data-stu-id="25743-209">It saves a bit of time.</span></span>
- <span data-ttu-id="25743-210">说明当前区域性或固定区域性如何影响输出的文章应解释预期输出。</span><span class="sxs-lookup"><span data-stu-id="25743-210">Articles explaining how current culture or invariant culture affect output should explain the expected output.</span></span> <span data-ttu-id="25743-211">交互式 REPL（读取评估打印循环）在基于 Linux 的主机上运行。</span><span class="sxs-lookup"><span data-stu-id="25743-211">The interactive REPL (Read Evaluate Print Loop) runs on a Linux-based host.</span></span> <span data-ttu-id="25743-212">默认区域性和固定区域性在不同的操作系统和计算机上生成不同输出。</span><span class="sxs-lookup"><span data-stu-id="25743-212">The default culture, and the invariant culture produce different output on different operating systems and machines.</span></span> <span data-ttu-id="25743-213">本文应介绍 Windows、Linux 和 Mac 系统中的输出。</span><span class="sxs-lookup"><span data-stu-id="25743-213">The article should explain the output in Windows, Linux, and Mac systems.</span></span>

### <a name="when-to-exclude-expected-output-from-the-sample"></a><span data-ttu-id="25743-214">何时不在示例中包含预期输出</span><span class="sxs-lookup"><span data-stu-id="25743-214">When to exclude expected output from the sample</span></span> 

- <span data-ttu-id="25743-215">示例生成较大输出的文章不应在注释中包含该输出。</span><span class="sxs-lookup"><span data-stu-id="25743-215">Articles where the sample generates a larger output should not include that in comments.</span></span> <span data-ttu-id="25743-216">运行该示例后，它会遮盖代码。</span><span class="sxs-lookup"><span data-stu-id="25743-216">It obscures the code once the sample has been run.</span></span>
- <span data-ttu-id="25743-217">示例演示一个主题但输出并不是理解它的必要条件的文章。</span><span class="sxs-lookup"><span data-stu-id="25743-217">Articles where the sample demonstrates a topic, but the output isn't integral to understanding it.</span></span> <span data-ttu-id="25743-218">例如，运行 LINQ 查询来解释查询语法，然后显示输出集合中的每个项的代码。</span><span class="sxs-lookup"><span data-stu-id="25743-218">For example, code that runs a LINQ query to explain query syntax and then display every item in the output collection.</span></span>

## <a name="dos-and-donts"></a><span data-ttu-id="25743-219">注意事项</span><span class="sxs-lookup"><span data-stu-id="25743-219">DOs and DON'Ts</span></span>

<span data-ttu-id="25743-220">以下列表显示了一些指导规则，当你参与 .NET 文档时应牢记其中的内容：</span><span class="sxs-lookup"><span data-stu-id="25743-220">The following list shows some guiding rules that you should keep in mind when you're contributing to the .NET documentation:</span></span>

- <span data-ttu-id="25743-221">请勿发出大型拉取请求。</span><span class="sxs-lookup"><span data-stu-id="25743-221">**DON'T** surprise us with large pull requests.</span></span> <span data-ttu-id="25743-222">可以提出问题并发起讨论，以便我们在你花费大量时间前确定方向。</span><span class="sxs-lookup"><span data-stu-id="25743-222">Instead, file an issue and start a discussion so we can agree on a direction before you invest a large amount of time.</span></span>
- <span data-ttu-id="25743-223">请务必阅读[风格指南](./styleguide/template.md)以及[语气和语调](./styleguide/voice-tone.md)指南。</span><span class="sxs-lookup"><span data-stu-id="25743-223">**DO** read the [style guide](./styleguide/template.md) and [voice and tone](./styleguide/voice-tone.md) guidelines.</span></span>
- <span data-ttu-id="25743-224">请务必使用[模板](./styleguide/template.md)文件作为工作的起点。</span><span class="sxs-lookup"><span data-stu-id="25743-224">**DO** use the [template](./styleguide/template.md) file as the starting point of your work.</span></span>
- <span data-ttu-id="25743-225">请务必在处理文章前，在分叉上创建一个单独的分支。</span><span class="sxs-lookup"><span data-stu-id="25743-225">**DO** create a separate branch on your fork before working on the articles.</span></span>
- <span data-ttu-id="25743-226">请务必遵循 [GitHub 流工作流](https://guides.github.com/introduction/flow/)。</span><span class="sxs-lookup"><span data-stu-id="25743-226">**DO** follow the [GitHub Flow workflow](https://guides.github.com/introduction/flow/).</span></span>
- <span data-ttu-id="25743-227">请务必在博客和推文（或任何社交软件上）频繁地发布你的参与内容！</span><span class="sxs-lookup"><span data-stu-id="25743-227">**DO** blog and tweet (or whatever) about your contributions, frequently!</span></span>

> <span data-ttu-id="25743-228">注意：你或许会注意到某些主题目前并没有遵循此处指定的所有准则和[风格指南](./styleguide/template.md)。</span><span class="sxs-lookup"><span data-stu-id="25743-228">Note: you might notice that some of the topics are not currently following all the guidelines specified here and on the [style guide](./styleguide/template.md) as well.</span></span> <span data-ttu-id="25743-229">我们正努力实现整个站点的一致性。</span><span class="sxs-lookup"><span data-stu-id="25743-229">We're working towards achieving consistency throughout the site.</span></span> <span data-ttu-id="25743-230">请查看我们当前正在跟踪的有关此特定目标的[未解决问题](https://github.com/dotnet/docs/issues?q=is%3Aissue+is%3Aopen+label%3Aguidelines-adherence)列表。</span><span class="sxs-lookup"><span data-stu-id="25743-230">Check the list of [open issues](https://github.com/dotnet/docs/issues?q=is%3Aissue+is%3Aopen+label%3Aguidelines-adherence) we're currently tracking for that specific goal.</span></span>

## <a name="contributor-license-agreement"></a><span data-ttu-id="25743-231">贡献者许可协议</span><span class="sxs-lookup"><span data-stu-id="25743-231">Contributor License Agreement</span></span>

<span data-ttu-id="25743-232">在合并 PR 前，必须签署 [.NET Foundation 贡献许可协议 (CLA)](https://cla.dotnetfoundation.org)。</span><span class="sxs-lookup"><span data-stu-id="25743-232">You must sign the [.NET Foundation Contribution License Agreement (CLA)](https://cla.dotnetfoundation.org) before your PR is merged.</span></span> <span data-ttu-id="25743-233">对于 .NET Foundation 中的项目，只需签署一次即可。</span><span class="sxs-lookup"><span data-stu-id="25743-233">This is a one-time requirement for projects in the .NET Foundation.</span></span> <span data-ttu-id="25743-234">可在维基百科上详细了解[贡献许可协议 (CLA)](http://en.wikipedia.org/wiki/Contributor_License_Agreement)。</span><span class="sxs-lookup"><span data-stu-id="25743-234">You can read more about [Contribution License Agreements (CLA)](http://en.wikipedia.org/wiki/Contributor_License_Agreement) on Wikipedia.</span></span>

<span data-ttu-id="25743-235">协议：[net-foundation-contribution-license-agreement.pdf](https://github.com/dotnet/home/blob/master/guidance/net-foundation-contribution-license-agreement.pdf)</span><span class="sxs-lookup"><span data-stu-id="25743-235">The agreement: [net-foundation-contribution-license-agreement.pdf](https://github.com/dotnet/home/blob/master/guidance/net-foundation-contribution-license-agreement.pdf)</span></span>

<span data-ttu-id="25743-236">无需事先签署该协议。</span><span class="sxs-lookup"><span data-stu-id="25743-236">You don't have to sign the agreement up-front.</span></span> <span data-ttu-id="25743-237">可如常克隆、创建分支并提交 PR。</span><span class="sxs-lookup"><span data-stu-id="25743-237">You can clone, fork, and submit your PR as usual.</span></span> <span data-ttu-id="25743-238">创建 PR 后，将由 CLA 自动程序对其分类。</span><span class="sxs-lookup"><span data-stu-id="25743-238">When your PR is created, it is classified by a CLA bot.</span></span> <span data-ttu-id="25743-239">如果更改的内容十分琐碎（如修复了拼写错误），则 PR 会被标记为 `cla-not-required`。</span><span class="sxs-lookup"><span data-stu-id="25743-239">If the change is trivial (for example, you fixed a typo), then the PR is labeled with `cla-not-required`.</span></span> <span data-ttu-id="25743-240">其他情况下，会分类为 `cla-required`。</span><span class="sxs-lookup"><span data-stu-id="25743-240">Otherwise, it's classified as `cla-required`.</span></span> <span data-ttu-id="25743-241">签署 CLA 后，当前和所有未来的拉取请求都会被标记为 `cla-signed`。</span><span class="sxs-lookup"><span data-stu-id="25743-241">Once you signed the CLA, the current and all future pull requests are labeled as `cla-signed`.</span></span>