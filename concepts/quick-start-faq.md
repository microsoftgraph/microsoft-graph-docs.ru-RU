---
title: 'Краткое руководство по Microsoft Graph: вопросы и ответы'
description: В этой статье представлены ответы на вопросы, связанные с краткими руководствами по Microsoft Graph.
author: jasonjoh
ms.author: jasonjoh
ms.date: 12/13/2018
localization_priority: Normal
ms.openlocfilehash: 457b82813420b8771a5e59e9723f11885388c7b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834946"
---
# <a name="microsoft-graph-quick-start-faq"></a><span data-ttu-id="ae737-103">Краткое руководство по Microsoft Graph: вопросы и ответы</span><span class="sxs-lookup"><span data-stu-id="ae737-103">Microsoft Graph quick start FAQ</span></span>

<span data-ttu-id="ae737-104">В этой статье представлены ответы на вопросы, связанные с [краткими руководствами по Microsoft Graph](https://developer.microsoft.com/graph/quick-start).</span><span class="sxs-lookup"><span data-stu-id="ae737-104">This FAQ answers questions related to the [Microsoft Graph Quick Starts](https://developer.microsoft.com/graph/quick-start).</span></span>

## <a name="general-design"></a><span data-ttu-id="ae737-105">Общая схема</span><span class="sxs-lookup"><span data-stu-id="ae737-105">General design</span></span>

<span data-ttu-id="ae737-106">В примерах, содержащихся в кратких руководствах, показано, как использовать всю мощь Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ae737-106">The quick start samples show you how to access the power of Microsoft Graph.</span></span> <span data-ttu-id="ae737-107">В этих примерах выполняется доступ к двум службам с использованием одной проверки подлинности: к учетной записи Майкрософт и Outlook.</span><span class="sxs-lookup"><span data-stu-id="ae737-107">These samples access two services with one authentication: Microsoft account and Outlook.</span></span> <span data-ttu-id="ae737-108">В каждом кратком руководстве используются сведения из профилей пользователей с учетными записями Майкрософт и отображаются события из их календаря.</span><span class="sxs-lookup"><span data-stu-id="ae737-108">Each quick start accesses information from Microsoft account users' profiles and displays events from their calendar.</span></span>

<span data-ttu-id="ae737-109">В каждом кратком руководстве необходимо выполнить четыре действия:</span><span class="sxs-lookup"><span data-stu-id="ae737-109">The quick starts involve four steps:</span></span>

- <span data-ttu-id="ae737-110">выбрать необходимую платформу;</span><span class="sxs-lookup"><span data-stu-id="ae737-110">Select your platform</span></span>
- <span data-ttu-id="ae737-111">получить идентификатор приложения (идентификатор клиента);</span><span class="sxs-lookup"><span data-stu-id="ae737-111">Get your app ID (client ID)</span></span>
- <span data-ttu-id="ae737-112">выполнить сборку кода из примера;</span><span class="sxs-lookup"><span data-stu-id="ae737-112">Build the sample</span></span>
- <span data-ttu-id="ae737-113">войти и просмотреть события в своем календаре.</span><span class="sxs-lookup"><span data-stu-id="ae737-113">Sign in, and view events on your calendar</span></span>

<span data-ttu-id="ae737-114">В итоге вы получите приложение, готовое к запуску.</span><span class="sxs-lookup"><span data-stu-id="ae737-114">When you complete the quick start, you have an app that's ready to run.</span></span>

## <a name="general-quick-start-sample-questions"></a><span data-ttu-id="ae737-115">Общие вопросы, касающиеся примеров из краткого руководства</span><span class="sxs-lookup"><span data-stu-id="ae737-115">General quick start sample questions</span></span>

<!-- markdownlint-disable MD026 -->

<span data-ttu-id="ae737-116">В этом разделе представлены ответы на вопросы о содержимом примеров из краткого руководства.</span><span class="sxs-lookup"><span data-stu-id="ae737-116">This section answers questions about the contents of the quick start samples.</span></span>

### <a name="can-i-get-the-quick-start-code-without-downloading-through-the-quick-start-page"></a><span data-ttu-id="ae737-117">Можно ли получить код из краткого руководства, не выполняя скачивание на странице краткого руководства?</span><span class="sxs-lookup"><span data-stu-id="ae737-117">Can I get the quick start code without downloading through the quick start page?</span></span>

<span data-ttu-id="ae737-118">Да, конечно!</span><span class="sxs-lookup"><span data-stu-id="ae737-118">Absolutely!</span></span> <span data-ttu-id="ae737-119">Каждый скачиваемый экземпляр краткого руководства основан на [учебнике по Microsoft Graph](tutorials.md), поэтому у вас есть два других варианта для получения такого же исходного кода:</span><span class="sxs-lookup"><span data-stu-id="ae737-119">Each quick start download is based on a [Microsoft Graph tutorial](tutorials.md), so you have two other options to get the same source code:</span></span>

- <span data-ttu-id="ae737-120">Выполнить сборку кода самостоятельно, следуя пошаговым инструкциям из учебника.</span><span class="sxs-lookup"><span data-stu-id="ae737-120">Build the code yourself by following the step-by-step tutorial.</span></span>
- <span data-ttu-id="ae737-121">Скачать готовый проект из соответствующего репозитория GitHub и выполнить инструкции из файла сведений, чтобы настроить и запустить пример.</span><span class="sxs-lookup"><span data-stu-id="ae737-121">Download the completed project from the corresponding GitHub repository and follow the instructions in the README to configure and run the sample.</span></span>

> <span data-ttu-id="ae737-122">**Примечание.** Мы работаем над созданием учебников для всех платформ, у которых в настоящее время есть краткие руководства.</span><span class="sxs-lookup"><span data-stu-id="ae737-122">**Note:** We are in the process of generating tutorials for each of the platforms that currently have a quick start.</span></span> <span data-ttu-id="ae737-123">Для некоторых кратких руководств пока нет соответствующих учебников.</span><span class="sxs-lookup"><span data-stu-id="ae737-123">Some of the quick starts do not have corresponding tutorials yet.</span></span>

#### <a name="tutorials-and-github-repositories"></a><span data-ttu-id="ae737-124">Учебники и репозитории GitHub</span><span class="sxs-lookup"><span data-stu-id="ae737-124">Tutorials and GitHub repositories</span></span>

<span data-ttu-id="ae737-125">В таблице ниже перечислены соответствующие учебники и репозитории GitHub для каждого примера из краткого руководства.</span><span class="sxs-lookup"><span data-stu-id="ae737-125">The following table lists the corresponding tutorial and GitHub repository for each quick start sample.</span></span>

| <span data-ttu-id="ae737-126">Краткое руководство</span><span class="sxs-lookup"><span data-stu-id="ae737-126">Quick start</span></span> | <span data-ttu-id="ae737-127">Учебник</span><span class="sxs-lookup"><span data-stu-id="ae737-127">Tutorial</span></span> | <span data-ttu-id="ae737-128">Репозиторий GitHub</span><span class="sxs-lookup"><span data-stu-id="ae737-128">GitHub repository</span></span> |
|-------------|----------|-------------------|
| <span data-ttu-id="ae737-129">Android</span><span class="sxs-lookup"><span data-stu-id="ae737-129">Android</span></span> | <span data-ttu-id="ae737-130">Нет</span><span class="sxs-lookup"><span data-stu-id="ae737-130">None</span></span> | [<span data-ttu-id="ae737-131">GitHub</span><span class="sxs-lookup"><span data-stu-id="ae737-131">GitHub</span></span>](https://github.com/microsoftgraph/android-java-connect-sample) |
| <span data-ttu-id="ae737-132">Angular</span><span class="sxs-lookup"><span data-stu-id="ae737-132">Angular</span></span> | [<span data-ttu-id="ae737-133">Учебник</span><span class="sxs-lookup"><span data-stu-id="ae737-133">Tutorial</span></span>](/graph/tutorials/angular) | [<span data-ttu-id="ae737-134">GitHub</span><span class="sxs-lookup"><span data-stu-id="ae737-134">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-angularspa) |
| <span data-ttu-id="ae737-135">ASP.NET MVC</span><span class="sxs-lookup"><span data-stu-id="ae737-135">ASP.NET MVC</span></span> | [<span data-ttu-id="ae737-136">Учебник</span><span class="sxs-lookup"><span data-stu-id="ae737-136">Tutorial</span></span>](/graph/tutorials/aspnet) | [<span data-ttu-id="ae737-137">GitHub</span><span class="sxs-lookup"><span data-stu-id="ae737-137">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-aspnetmvcapp) |
| <span data-ttu-id="ae737-138">iOS Swift</span><span class="sxs-lookup"><span data-stu-id="ae737-138">iOS Swift</span></span> | <span data-ttu-id="ae737-139">Нет</span><span class="sxs-lookup"><span data-stu-id="ae737-139">None</span></span> | [<span data-ttu-id="ae737-140">GitHub</span><span class="sxs-lookup"><span data-stu-id="ae737-140">GitHub</span></span>](https://github.com/microsoftgraph/ios-swift-connect-sample) |
| <span data-ttu-id="ae737-141">iOS Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae737-141">iOS Objective-C</span></span> | <span data-ttu-id="ae737-142">Нет</span><span class="sxs-lookup"><span data-stu-id="ae737-142">None</span></span> | [<span data-ttu-id="ae737-143">GitHub</span><span class="sxs-lookup"><span data-stu-id="ae737-143">GitHub</span></span>](https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample) |
| <span data-ttu-id="ae737-144">Node.js</span><span class="sxs-lookup"><span data-stu-id="ae737-144">Node.js</span></span> | [<span data-ttu-id="ae737-145">Учебник</span><span class="sxs-lookup"><span data-stu-id="ae737-145">Tutorial</span></span>](/graph/tutorials/node) | [<span data-ttu-id="ae737-146">GitHub</span><span class="sxs-lookup"><span data-stu-id="ae737-146">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-nodeexpressapp) |
| <span data-ttu-id="ae737-147">PHP</span><span class="sxs-lookup"><span data-stu-id="ae737-147">PHP</span></span> | [<span data-ttu-id="ae737-148">Учебник</span><span class="sxs-lookup"><span data-stu-id="ae737-148">Tutorial</span></span>](/graph/tutorials/php) | [<span data-ttu-id="ae737-149">GitHub</span><span class="sxs-lookup"><span data-stu-id="ae737-149">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-phpapp) |
| <span data-ttu-id="ae737-150">Python</span><span class="sxs-lookup"><span data-stu-id="ae737-150">Python</span></span> | [<span data-ttu-id="ae737-151">Учебник</span><span class="sxs-lookup"><span data-stu-id="ae737-151">Tutorial</span></span>](/graph/tutorials/python) | [<span data-ttu-id="ae737-152">GitHub</span><span class="sxs-lookup"><span data-stu-id="ae737-152">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-pythondjangoapp) |
| <span data-ttu-id="ae737-153">Ruby</span><span class="sxs-lookup"><span data-stu-id="ae737-153">Ruby</span></span> | [<span data-ttu-id="ae737-154">Учебник</span><span class="sxs-lookup"><span data-stu-id="ae737-154">Tutorial</span></span>](/graph/tutorials/ruby) | [<span data-ttu-id="ae737-155">GitHub</span><span class="sxs-lookup"><span data-stu-id="ae737-155">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-rubyrailsapp) |
| <span data-ttu-id="ae737-156">UWP</span><span class="sxs-lookup"><span data-stu-id="ae737-156">UWP</span></span> | [<span data-ttu-id="ae737-157">Учебник</span><span class="sxs-lookup"><span data-stu-id="ae737-157">Tutorial</span></span>](/graph/tutorials/uwp) | [<span data-ttu-id="ae737-158">GitHub</span><span class="sxs-lookup"><span data-stu-id="ae737-158">GitHub</span></span>](https://github.com/microsoftgraph/msgraph-training-uwp) |
| <span data-ttu-id="ae737-159">Xamarin</span><span class="sxs-lookup"><span data-stu-id="ae737-159">Xamarin</span></span> | <span data-ttu-id="ae737-160">Нет</span><span class="sxs-lookup"><span data-stu-id="ae737-160">None</span></span> | [<span data-ttu-id="ae737-161">GitHub</span><span class="sxs-lookup"><span data-stu-id="ae737-161">GitHub</span></span>](https://github.com/microsoftgraph/xamarin-csharp-connect-sample) |

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a><span data-ttu-id="ae737-162">Почему в примерах из краткого руководства нет вариантов использования расширенной проверки подлинности?</span><span class="sxs-lookup"><span data-stu-id="ae737-162">Why don't any of the quick start samples show advanced authentication use cases?</span></span>

<span data-ttu-id="ae737-163">Примеры из краткого руководства используются для ознакомления с функцией проверки подлинности и вызовов API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ae737-163">The quick start samples give you an introduction to authentication and Microsoft Graph API calls.</span></span> <span data-ttu-id="ae737-164">Дополнительные сведения о других потоках проверки подлинности см. в документации [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios).</span><span class="sxs-lookup"><span data-stu-id="ae737-164">You can learn more about other authentication flows in the [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios) documentation.</span></span>

### <a name="what-if-i-run-into-an-unexpected-error-or-problem-with-a-quick-start"></a><span data-ttu-id="ae737-165">Что делать при возникновении непредвиденной ошибки или проблемы с кратким руководством?</span><span class="sxs-lookup"><span data-stu-id="ae737-165">What if I run into an unexpected error or problem with a quick start?</span></span>

<span data-ttu-id="ae737-166">Если не удается обеспечить правильную работу при использовании краткого руководства, опубликуйте проблему в соответствующем репозитории GitHub.</span><span class="sxs-lookup"><span data-stu-id="ae737-166">If you have trouble getting the quick start to work properly, please open an issue on the corresponding GitHub repository.</span></span>

## <a name="didnt-find-what-you-need"></a><span data-ttu-id="ae737-167">Не нашли то, что искали?</span><span class="sxs-lookup"><span data-stu-id="ae737-167">Didn't find what you need?</span></span>

<span data-ttu-id="ae737-168">Если в этой статье вы не нашли ответ на интересующий вас вопрос касательно одного или нескольких кратких руководств, сообщите нам об этом в разделе **Отзыв** ниже.</span><span class="sxs-lookup"><span data-stu-id="ae737-168">If this FAQ didn't address a question or problem you encountered with one or more of the quick starts, please let us know using the **Feedback** section below.</span></span>
