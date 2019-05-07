---
title: Развертывание, тестирование и расширение перенесенных приложений
description: 'В этой статье описывается перенос приложений Azure Active Directory (Azure AD) для использования API Microsoft Graph (REST); в этом разделе описывается шаг 3: развертывание, тестирование и расширение.'
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8a63c14ef27648a1d586551ebe12e18a5f263a9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630253"
---
# <a name="deploy-test-and-extend"></a><span data-ttu-id="27433-103">Развертывание, тестирование и расширение</span><span class="sxs-lookup"><span data-stu-id="27433-103">Deploy, test, and extend</span></span>

<span data-ttu-id="27433-104">Это шаг 4 [процесса миграции приложений](migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="27433-104">This is step 4 of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

1.  <span data-ttu-id="27433-105">**Тестирование**</span><span class="sxs-lookup"><span data-stu-id="27433-105">**Test throughly**</span></span>

    <span data-ttu-id="27433-106">После обновления приложения тщательно протестируйте его, чтобы убедиться, что он работает должным образом и что вы не предоставили какие-либо регрессе.</span><span class="sxs-lookup"><span data-stu-id="27433-106">Once you've updated your app, test it thoroughly to verify that it works as expected and that you haven't introduced any regressions.</span></span>  

    <span data-ttu-id="27433-107">Обязательно используйте несколько сред, наборов данных и персонажей для конечных пользователей, например, учетные данные с разными ролями, правами и обязанностями.</span><span class="sxs-lookup"><span data-stu-id="27433-107">Be sure to use multiple environments, data sets, and end-user personas, e.g. credentials with different roles, rights, and responsibilities.</span></span> <span data-ttu-id="27433-108">Пройдите весь жизненный цикл, получив новый тестовый пользователь в первый раз, а также существующего пользователя (который уже был отправлен), пытающегося повторно использовать приложение.</span><span class="sxs-lookup"><span data-stu-id="27433-108">Go through the entire lifecycle, by having a new test user acquire the app for the first time, as well as an existing user (who already consented) trying to use the app again.</span></span>

2.  <span data-ttu-id="27433-109">**Развертывание поэтапных обновлений**</span><span class="sxs-lookup"><span data-stu-id="27433-109">**Deploy staged updates**</span></span>

    <span data-ttu-id="27433-110">Рекомендуется развертывать обновления поэтапно.</span><span class="sxs-lookup"><span data-stu-id="27433-110">Consider deploying your updates in stages.</span></span>  <span data-ttu-id="27433-111">Ограниченное развертывание с небольшим набором понятных пользователей помогает выявить проблемы и другие проблемы, связанные с потенциальным вредом.</span><span class="sxs-lookup"><span data-stu-id="27433-111">A limited roll-out to a small set of friendly users can help identify glitches and other potentially-embarrassing issues.</span></span>  <span data-ttu-id="27433-112">Это также дает возможность отслеживать первоначальный прием и обратную связь.</span><span class="sxs-lookup"><span data-stu-id="27433-112">This also gives you a chance to monitor initial reception and feedback.</span></span>

    <span data-ttu-id="27433-113">Если первоначальное развертывание хорошо продвигается, проследите за ходом развертывания в крупных аудиториях.</span><span class="sxs-lookup"><span data-stu-id="27433-113">If the initial roll-out goes well, monitor progress as you deploy to larger audiences.</span></span>

3.  <span data-ttu-id="27433-114">**Просмотр нового значения**</span><span class="sxs-lookup"><span data-stu-id="27433-114">**Explore new value**</span></span>

    <span data-ttu-id="27433-115">Теперь, когда вы переключились на Microsoft Graph, вы не сможете упростить разблокировку многих дополнительных наборов данных и функций, которые теперь доступны вам.</span><span class="sxs-lookup"><span data-stu-id="27433-115">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="27433-116">Регулярно проверяйте наличие новых наборов данных и возможностей.</span><span class="sxs-lookup"><span data-stu-id="27433-116">Check for new datasets and capabilities regularly.</span></span>  

    - <span data-ttu-id="27433-117">Ознакомьтесь с тем, [что можно делать с помощью Microsoft Graph](/graph/examples) .</span><span class="sxs-lookup"><span data-stu-id="27433-117">Take a look at [what you can do with Microsoft Graph](/graph/examples)</span></span>
    - <span data-ttu-id="27433-118">В [блоге Microsoft Graph](/graph/blogs) вы узнаете о последних новостях о Microsoft Graph и некоторых полезных циклах обучения.</span><span class="sxs-lookup"><span data-stu-id="27433-118">Explore the [Microsoft Graph blog](/graph/blogs) for the latest news about Microsoft Graph and some great learning series.</span></span>
    - <span data-ttu-id="27433-119">Журнал [изменений](/greaph/changelog) содержит сведения об обновлениях служб и документов.</span><span class="sxs-lookup"><span data-stu-id="27433-119">The [changelog](/greaph/changelog) summarizes service and document updates.</span></span> <span data-ttu-id="27433-120">Следуя этим обновлениям, вы можете отслеживать новые API, введенные в/Beta (Предварительная версия), и те, которые продвинулись до версии 1.0 (GA).</span><span class="sxs-lookup"><span data-stu-id="27433-120">Following these updates will help you track new APIs introduced to /beta (preview) and those promoted to v1.0 (GA).</span></span>  <span data-ttu-id="27433-121">Эти новые API могут предоставить новые способы добавления новых значений и новых возможностей в ваши приложения.</span><span class="sxs-lookup"><span data-stu-id="27433-121">These new APIs can provide new ways for you to add more value and new experiences to your apps.</span></span>  

## <a name="see-also"></a><span data-ttu-id="27433-122">См. также</span><span class="sxs-lookup"><span data-stu-id="27433-122">See also</span></span>

<span data-ttu-id="27433-123">Если во время миграции возникают проблемы или необходима помощь, можно выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="27433-123">If you run into problems or need help during the migration process, you can:</span></span>

- <span data-ttu-id="27433-124">Повторное изучение [контрольного списка](migrate-azure-ad-graph-overview.md)</span><span class="sxs-lookup"><span data-stu-id="27433-124">Review the [checklist](migrate-azure-ad-graph-overview.md) again</span></span>
- <span data-ttu-id="27433-125">Отправка вопросов в [сайте StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph)</span><span class="sxs-lookup"><span data-stu-id="27433-125">Post questions to [StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph)</span></span>
- <span data-ttu-id="27433-126">Просмотрите примеры Microsoft Graph и сравните их с существующим кодом приложения:</span><span class="sxs-lookup"><span data-stu-id="27433-126">Review Microsoft Graph samples to contrast and compare with your existing application code:</span></span>
  - <span data-ttu-id="27433-127">**Приложения, ИСПОЛЬЗУЮЩИЕ REST API**: краткие [руководства по началу работы и примеры](/graph/get-started), выбор вашей платформы и запуск с помощью краткого руководства или поиск подходящего примера</span><span class="sxs-lookup"><span data-stu-id="27433-127">**Apps that use the REST API**: explore [quick starts and samples](/graph/get-started), choosing your platform of choice and run through the quick start or search for an appropriate sample</span></span>
  - <span data-ttu-id="27433-128">**Приложение, использующее клиентскую библиотеку .NET**: "Рецензирование", " [консоль CSharp-сниппетов-фрагменты-Sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) " и/или [дотнеткоре-Console-Sample](https://github.com/microsoftgraph/dotnetcore-console-sample)</span><span class="sxs-lookup"><span data-stu-id="27433-128">**App that use the .NET client library**: review [console-csharp-snippets-sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) and/or [dotnetcore-console-sample](https://github.com/microsoftgraph/dotnetcore-console-sample)</span></span>

## <a name="next-steps"></a><span data-ttu-id="27433-129">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="27433-129">Next Steps</span></span>

- <span data-ttu-id="27433-130">Используйте [быстрые запуски и примеры](/graph/get-started) для ускорения.</span><span class="sxs-lookup"><span data-stu-id="27433-130">Use [quick starts and samples](/graph/get-started) to come up to speed quickly.</span></span>
- <span data-ttu-id="27433-131">Использование [клиентских библиотек и пакетов SDK](https://developer.microsoft.com/graph/get-started) для разработки пользовательских приложений</span><span class="sxs-lookup"><span data-stu-id="27433-131">Leverage [client libraries and SDKs](https://developer.microsoft.com/graph/get-started) to develop custom applications</span></span> 
- <span data-ttu-id="27433-132">Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .</span><span class="sxs-lookup"><span data-stu-id="27433-132">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="27433-133">Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .</span><span class="sxs-lookup"><span data-stu-id="27433-133">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
