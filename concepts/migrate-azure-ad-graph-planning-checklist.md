---
title: Контрольный список планирования миграции приложений
description: Контрольный список для переноса приложений из Azure AD Graph в Microsoft Graph
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 905a692e6a4fddf71b6488e1695957cba5b182ae
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778266"
---
# <a name="app-migration-planning-checklist"></a><span data-ttu-id="ee7a9-103">Контрольный список планирования миграции приложений</span><span class="sxs-lookup"><span data-stu-id="ee7a9-103">App migration planning checklist</span></span>

<span data-ttu-id="ee7a9-104">Используйте следующий контрольный список для планирования миграции:</span><span class="sxs-lookup"><span data-stu-id="ee7a9-104">Use the following checklist to plan your migration:</span></span>

## <a name="step-1-review-the-differences-between-the-apis"></a><span data-ttu-id="ee7a9-105">Шаг 1: Ознакомьтесь с различиями между API</span><span class="sxs-lookup"><span data-stu-id="ee7a9-105">Step 1: Review the differences between the APIs</span></span>

<span data-ttu-id="ee7a9-106">Во многих отношениях Microsoft Graph аналогичен более ранней версии Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="ee7a9-106">In many respects, Microsoft Graph is similar to the earlier Azure AD Graph.</span></span> <span data-ttu-id="ee7a9-107">Во многих случаях просто измените имя и версию службы конечных точек в коде, и все должно продолжать работу.</span><span class="sxs-lookup"><span data-stu-id="ee7a9-107">In many cases, simply change the endpoint service name and version in your code, and everything should continue to work.</span></span>

<span data-ttu-id="ee7a9-108">Тем не менее, существуют различия.</span><span class="sxs-lookup"><span data-stu-id="ee7a9-108">Nonetheless, there are differences.</span></span> <span data-ttu-id="ee7a9-109">Изменены некоторые ресурсы, свойства, методы и основные возможности.</span><span class="sxs-lookup"><span data-stu-id="ee7a9-109">Certain resources, properties, methods, and core capabilities have changed.</span></span>

<span data-ttu-id="ee7a9-110">В частности, ищите различия в следующих областях:</span><span class="sxs-lookup"><span data-stu-id="ee7a9-110">Specifically, look for differences in the following areas:</span></span>

- <span data-ttu-id="ee7a9-111">[Синтаксис запроса на вызов](migrate-azure-ad-graph-request-differences.md) между двумя службами</span><span class="sxs-lookup"><span data-stu-id="ee7a9-111">[Request call syntax](migrate-azure-ad-graph-request-differences.md) between the two services</span></span>
- <span data-ttu-id="ee7a9-112">[Различия](migrate-azure-ad-graph-feature-differences.md)в функциях, такие как расширения каталогов, пакетная обработка, разностные запросы и т. д.</span><span class="sxs-lookup"><span data-stu-id="ee7a9-112">[Feature differences](migrate-azure-ad-graph-feature-differences.md), such as directory extensions, batching, differential queries, and so on</span></span>
- <span data-ttu-id="ee7a9-113">[Имена ресурсов сущностей](migrate-azure-ad-graph-resource-differences.md) и их типы</span><span class="sxs-lookup"><span data-stu-id="ee7a9-113">[Entity resource names](migrate-azure-ad-graph-resource-differences.md) and their types</span></span>
- <span data-ttu-id="ee7a9-114">[Свойства](migrate-azure-ad-graph-property-differences.md) объектов Request и Response</span><span class="sxs-lookup"><span data-stu-id="ee7a9-114">[Properties](migrate-azure-ad-graph-property-differences.md) of request and response objects</span></span>
- <span data-ttu-id="ee7a9-115">[Методы](migrate-azure-ad-graph-method-differences.md), включая параметры и типы</span><span class="sxs-lookup"><span data-stu-id="ee7a9-115">[Methods](migrate-azure-ad-graph-method-differences.md), including parameters and types</span></span>

## <a name="step-2-examine-api-use"></a><span data-ttu-id="ee7a9-116">Шаг 2: Проверка использования API</span><span class="sxs-lookup"><span data-stu-id="ee7a9-116">Step 2: Examine API use</span></span>

<span data-ttu-id="ee7a9-117">[Изучите API](migrate-azure-ad-graph-audit-api-use.md) , используемые вашим приложением, необходимые разрешения и сравните со списком известных отличий.</span><span class="sxs-lookup"><span data-stu-id="ee7a9-117">[Examine the APIs](migrate-azure-ad-graph-audit-api-use.md) used by your app, the permissions they require, and compare to the list of known differences.</span></span>  

<span data-ttu-id="ee7a9-118">Убедитесь, что нужные API-интерфейсы, как правило, доступны в Microsoft Graph версии 1.0, и что эти API работают одинаковым образом.</span><span class="sxs-lookup"><span data-stu-id="ee7a9-118">Verify that the APIs your app needs are generally available in Microsoft Graph v1.0 and that these APIs work the same way.</span></span>

<span data-ttu-id="ee7a9-119">В некоторых случаях новые возможности и функции предназначены для замены более ранних подходов.</span><span class="sxs-lookup"><span data-stu-id="ee7a9-119">In some cases, new capabilities and features are designed to replace earlier approaches.</span></span>

<span data-ttu-id="ee7a9-120">Используйте [проводник Graph](https://aka.ms/ge) для экспериментов с новыми вызовами и разработки новых подходов.</span><span class="sxs-lookup"><span data-stu-id="ee7a9-120">Use the [Graph Explorer](https://aka.ms/ge) to experiment with new calls and to develop new approaches.</span></span> <span data-ttu-id="ee7a9-121">Для достижения лучших результатов Войдите в систему, используя учетные данные тестового пользователя в тестовом клиенте, чтобы увидеть, что API выполняет над важными наборами данных.</span><span class="sxs-lookup"><span data-stu-id="ee7a9-121">For best results, sign in using the credentials of a test user in a test tenant so that you see what the API does over important data sets.</span></span>

## <a name="step-3-review-app-details"></a><span data-ttu-id="ee7a9-122">Шаг 3: Просмотр сведений о приложении</span><span class="sxs-lookup"><span data-stu-id="ee7a9-122">Step 3: Review app details</span></span>

- <span data-ttu-id="ee7a9-123">Изменения регистрации и согласия [приложения](migrate-azure-ad-graph-app-registration.md) (не должно быть None).</span><span class="sxs-lookup"><span data-stu-id="ee7a9-123">[App registration](migrate-azure-ad-graph-app-registration.md) and consent changes (which should be none).</span></span>
- <span data-ttu-id="ee7a9-124">Получение маркеров и [библиотек проверки](migrate-azure-ad-graph-authentication-library.md)подлинности.</span><span class="sxs-lookup"><span data-stu-id="ee7a9-124">Token acquisition and [authentication libraries](migrate-azure-ad-graph-authentication-library.md).</span></span>
- <span data-ttu-id="ee7a9-125">Для приложений .NET используйте клиентские [библиотеки](migrate-azure-ad-graph-client-libraries.md).</span><span class="sxs-lookup"><span data-stu-id="ee7a9-125">For .NET applications, use of [client libraries](migrate-azure-ad-graph-client-libraries.md).</span></span>

## <a name="step-4-deploy-test-and-extend-your-app"></a><span data-ttu-id="ee7a9-126">Шаг 4: развертывание, тестирование и расширение приложения</span><span class="sxs-lookup"><span data-stu-id="ee7a9-126">Step 4: Deploy, test, and extend your app</span></span>

<span data-ttu-id="ee7a9-127">Прежде чем обновлять приложение для всех пользователей, убедитесь, что вы тщательно протестируете и разработайте перед развертыванием вашей аудитории клиентов.</span><span class="sxs-lookup"><span data-stu-id="ee7a9-127">Before updating your app for everyone, ensure you test thoroughly and stage your rollout to your customer audience.</span></span>

<span data-ttu-id="ee7a9-128">Теперь, когда вы переключились на Microsoft Graph, вы не сможете упростить разблокировку многих дополнительных наборов данных и функций, которые теперь доступны вам.</span><span class="sxs-lookup"><span data-stu-id="ee7a9-128">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="ee7a9-129">Вы можете узнать о возможных возможностях, изучив некоторые [примеры](/graph/examples).</span><span class="sxs-lookup"><span data-stu-id="ee7a9-129">You can get a taste of what's possible by looking at some [examples](/graph/examples).</span></span>

<span data-ttu-id="ee7a9-130">Если вы используете [библиотеку проверки подлинности Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), рассмотрите возможность переключения на [библиотеку проверки подлинности Microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span><span class="sxs-lookup"><span data-stu-id="ee7a9-130">If you're currently using the [AD authentication library](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), consider switching to the [Microsoft authentication library](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span></span>

## <a name="next-steps"></a><span data-ttu-id="ee7a9-131">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="ee7a9-131">Next Steps</span></span>

- <span data-ttu-id="ee7a9-132">Сведения о [синтаксисе вызова рескуест](migrate-azure-ad-graph-request-differences.md) для начала действия 1: обзор различий API.</span><span class="sxs-lookup"><span data-stu-id="ee7a9-132">Learn about [resquest call syntax](migrate-azure-ad-graph-request-differences.md) to start step 1: reviewing API differences.</span></span>
- <span data-ttu-id="ee7a9-133">Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .</span><span class="sxs-lookup"><span data-stu-id="ee7a9-133">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="ee7a9-134">Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .</span><span class="sxs-lookup"><span data-stu-id="ee7a9-134">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
- <span data-ttu-id="ee7a9-135">Чтобы узнать больше об обновлениях хода выполнения и временных шкалах, ознакомьтесь со статьей [Microsoft Graph или Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) в центре разработчиков Office.</span><span class="sxs-lookup"><span data-stu-id="ee7a9-135">To learn more about progress updates and timelines, see [Microsoft Graph or the Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) in the Office Dev Center.</span></span>
