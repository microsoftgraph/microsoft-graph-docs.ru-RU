---
title: Контрольный список планирования миграции приложений
description: Контрольный список для переноса приложений из Azure AD Graph в Microsoft Graph
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: f8e231166fdb39676ce2778b369c6962cae70cb0
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/16/2021
ms.locfileid: "49882747"
---
# <a name="app-migration-planning-checklist"></a><span data-ttu-id="81025-103">Контрольный список планирования миграции приложений</span><span class="sxs-lookup"><span data-stu-id="81025-103">App migration planning checklist</span></span>

> [!Important]
> <span data-ttu-id="81025-104">API Graph Azure AD теперь является неподготовленным.</span><span class="sxs-lookup"><span data-stu-id="81025-104">Azure AD Graph API is now deprecated.</span></span> <span data-ttu-id="81025-105">Мы продолжим предоставлять техническую поддержку и обновления для системы безопасности, но больше не будем предоставлять обновления функций.</span><span class="sxs-lookup"><span data-stu-id="81025-105">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
> <span data-ttu-id="81025-106">Начиная с 30 июня 2022 г., поддержка Azure AD Graph будет прекратиться и мы больше не будем предоставлять техническую поддержку или обновления для системы безопасности.</span><span class="sxs-lookup"><span data-stu-id="81025-106">Starting June 30th, 2022, we will end support for Azure AD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="81025-107">После этого приложения, использующие Azure AD Graph, больше не будут получать ответы от конечной точки Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="81025-107">Apps using Azure AD Graph after this time will no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="81025-108">Используйте следующий контрольный список для планирования миграции.</span><span class="sxs-lookup"><span data-stu-id="81025-108">Use the following checklist to plan your migration.</span></span>

## <a name="step-1-review-the-differences-between-the-apis"></a><span data-ttu-id="81025-109">Шаг 1. Просмотр различий между API</span><span class="sxs-lookup"><span data-stu-id="81025-109">Step 1: Review the differences between the APIs</span></span>

<span data-ttu-id="81025-110">Во многом Microsoft Graph похож на предыдущий Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="81025-110">In many respects, Microsoft Graph is similar to the earlier Azure AD Graph.</span></span> <span data-ttu-id="81025-111">Во многих случаях просто измените имя и версию службы конечной точки в коде, и все должно работать.</span><span class="sxs-lookup"><span data-stu-id="81025-111">In many cases, simply change the endpoint service name and version in your code, and everything should continue to work.</span></span>

<span data-ttu-id="81025-112">Тем не менее, существуют различия.</span><span class="sxs-lookup"><span data-stu-id="81025-112">Nonetheless, there are differences.</span></span> <span data-ttu-id="81025-113">Изменены некоторые ресурсы, свойства, методы и основные возможности.</span><span class="sxs-lookup"><span data-stu-id="81025-113">Certain resources, properties, methods, and core capabilities have changed.</span></span>

<span data-ttu-id="81025-114">В частности, следует искать различия в следующих областях:</span><span class="sxs-lookup"><span data-stu-id="81025-114">Specifically, look for differences in the following areas:</span></span>

- <span data-ttu-id="81025-115">[Запрос синтаксиса вызовов](migrate-azure-ad-graph-request-differences.md) между двумя службами</span><span class="sxs-lookup"><span data-stu-id="81025-115">[Request call syntax](migrate-azure-ad-graph-request-differences.md) between the two services</span></span>
- <span data-ttu-id="81025-116">[Отличия функций,](migrate-azure-ad-graph-feature-differences.md)такие как расширения каталогов, пакетная обработка, разнонаправленные запросы и так далее</span><span class="sxs-lookup"><span data-stu-id="81025-116">[Feature differences](migrate-azure-ad-graph-feature-differences.md), such as directory extensions, batching, differential queries, and so on</span></span>
- <span data-ttu-id="81025-117">[Имена ресурсов сущности и](migrate-azure-ad-graph-resource-differences.md) их типы</span><span class="sxs-lookup"><span data-stu-id="81025-117">[Entity resource names](migrate-azure-ad-graph-resource-differences.md) and their types</span></span>
- <span data-ttu-id="81025-118">[Свойства объектов](migrate-azure-ad-graph-property-differences.md) запросов и ответов</span><span class="sxs-lookup"><span data-stu-id="81025-118">[Properties](migrate-azure-ad-graph-property-differences.md) of request and response objects</span></span>
- <span data-ttu-id="81025-119">[Методы,](migrate-azure-ad-graph-method-differences.md)включая параметры и типы</span><span class="sxs-lookup"><span data-stu-id="81025-119">[Methods](migrate-azure-ad-graph-method-differences.md), including parameters and types</span></span>

## <a name="step-2-examine-api-use"></a><span data-ttu-id="81025-120">Шаг 2. Изучение использования API</span><span class="sxs-lookup"><span data-stu-id="81025-120">Step 2: Examine API use</span></span>

<span data-ttu-id="81025-121">[Проверьте API,](migrate-azure-ad-graph-audit-api-use.md) используемые вашим приложением, необходимые им разрешения, и сравните их со списком известных различий.</span><span class="sxs-lookup"><span data-stu-id="81025-121">[Examine the APIs](migrate-azure-ad-graph-audit-api-use.md) used by your app, the permissions they require, and compare to the list of known differences.</span></span>  

<span data-ttu-id="81025-122">Убедитесь, что API, необходимые вашему приложению, как правило, доступны в Microsoft Graph 1.0 и что эти API работают одинаково.</span><span class="sxs-lookup"><span data-stu-id="81025-122">Verify that the APIs your app needs are generally available in Microsoft Graph v1.0 and that these APIs work the same way.</span></span>

<span data-ttu-id="81025-123">В некоторых случаях новые возможности и функции предназначены для замены более ранних подходов.</span><span class="sxs-lookup"><span data-stu-id="81025-123">In some cases, new capabilities and features are designed to replace earlier approaches.</span></span>

<span data-ttu-id="81025-124">Используйте [обозреватель Graph для](https://aka.ms/ge) экспериментов с новыми вызовами и разработки новых подходов.</span><span class="sxs-lookup"><span data-stu-id="81025-124">Use the [Graph Explorer](https://aka.ms/ge) to experiment with new calls and to develop new approaches.</span></span> <span data-ttu-id="81025-125">Для наилучших результатов во sign in using the credentials of a test user in a test tenant so that you see what the API does over important data sets.</span><span class="sxs-lookup"><span data-stu-id="81025-125">For best results, sign in using the credentials of a test user in a test tenant so that you see what the API does over important data sets.</span></span>

## <a name="step-3-review-app-details"></a><span data-ttu-id="81025-126">Шаг 3. Просмотр сведений о приложении</span><span class="sxs-lookup"><span data-stu-id="81025-126">Step 3: Review app details</span></span>

- <span data-ttu-id="81025-127">[Изменения регистрации](migrate-azure-ad-graph-app-registration.md) и согласия приложения (которых не должно быть).</span><span class="sxs-lookup"><span data-stu-id="81025-127">[App registration](migrate-azure-ad-graph-app-registration.md) and consent changes (which should be none).</span></span>
- <span data-ttu-id="81025-128">Библиотеки получения маркеров [и проверки подлинности.](migrate-azure-ad-graph-authentication-library.md)</span><span class="sxs-lookup"><span data-stu-id="81025-128">Token acquisition and [authentication libraries](migrate-azure-ad-graph-authentication-library.md).</span></span>
- <span data-ttu-id="81025-129">Для приложений .NET используйте [клиентские библиотеки.](migrate-azure-ad-graph-client-libraries.md)</span><span class="sxs-lookup"><span data-stu-id="81025-129">For .NET applications, use of [client libraries](migrate-azure-ad-graph-client-libraries.md).</span></span>

## <a name="step-4-deploy-test-and-extend-your-app"></a><span data-ttu-id="81025-130">Шаг 4. Развертывание, тестирование и расширение приложения</span><span class="sxs-lookup"><span data-stu-id="81025-130">Step 4: Deploy, test, and extend your app</span></span>

<span data-ttu-id="81025-131">Перед обновлением приложения для всех убедитесь, что вы тщательно протестировали свое приложение и развяли его для аудитории клиента.</span><span class="sxs-lookup"><span data-stu-id="81025-131">Before updating your app for everyone, ensure you test thoroughly and stage your rollout to your customer audience.</span></span>

<span data-ttu-id="81025-132">Теперь, когда вы перешли на Microsoft Graph, вам никогда не было проще разблокировать намного больше наборов данных и функций, которые теперь находятся под рукой.</span><span class="sxs-lookup"><span data-stu-id="81025-132">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="81025-133">Вы можете получить опробуя возможности, изумив некоторые основные службы и [функции в Microsoft Graph.](./overview-major-services.md)</span><span class="sxs-lookup"><span data-stu-id="81025-133">You can get a taste of what's possible by looking at some of the [Major services and features in Microsoft Graph](./overview-major-services.md).</span></span>

<span data-ttu-id="81025-134">Если вы в настоящее время используете библиотеку проверки подлинности [AD](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), рассмотрите возможность перехода на библиотеку проверки подлинности [Майкрософт](/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span><span class="sxs-lookup"><span data-stu-id="81025-134">If you're currently using the [AD authentication library](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), consider switching to the [Microsoft authentication library](/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span></span>

## <a name="next-steps"></a><span data-ttu-id="81025-135">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="81025-135">Next Steps</span></span>

- <span data-ttu-id="81025-136">Узнайте о [синтаксис вызова](migrate-azure-ad-graph-request-differences.md) запроса для начала шага 1: просмотр различий API.</span><span class="sxs-lookup"><span data-stu-id="81025-136">Learn about [request call syntax](migrate-azure-ad-graph-request-differences.md) to start step 1: reviewing API differences.</span></span>