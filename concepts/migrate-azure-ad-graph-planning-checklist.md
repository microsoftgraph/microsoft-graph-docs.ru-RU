---
title: Контрольный список планирования миграции приложений
description: Контрольный список для переноса приложений из Azure AD Graph в Microsoft Graph
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: a61e5180194246bbea5cc32e42666beab83882fa
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761285"
---
# <a name="app-migration-planning-checklist"></a><span data-ttu-id="beedf-103">Контрольный список планирования миграции приложений</span><span class="sxs-lookup"><span data-stu-id="beedf-103">App migration planning checklist</span></span>

> [!Important]
> <span data-ttu-id="beedf-104">API Azure AD Graph теперь отстает.</span><span class="sxs-lookup"><span data-stu-id="beedf-104">Azure AD Graph API is now deprecated.</span></span> <span data-ttu-id="beedf-105">Мы продолжим предоставлять техническую поддержку и обновления для системы безопасности, но больше не будем предоставлять обновления компонентов.</span><span class="sxs-lookup"><span data-stu-id="beedf-105">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
> <span data-ttu-id="beedf-106">Начиная с 30 июня 2022 г. мы переимеем поддержку Azure AD Graph и больше не будем предоставлять техническую поддержку или обновления безопасности.</span><span class="sxs-lookup"><span data-stu-id="beedf-106">Starting June 30th, 2022, we will end support for Azure AD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="beedf-107">Приложения, использующие Azure AD Graph после этого времени, больше не будут получать ответы из конечной точки Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="beedf-107">Apps using Azure AD Graph after this time will no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="beedf-108">Чтобы спланировать миграцию, используйте следующий контрольный список.</span><span class="sxs-lookup"><span data-stu-id="beedf-108">Use the following checklist to plan your migration.</span></span>

## <a name="step-1-review-the-differences-between-the-apis"></a><span data-ttu-id="beedf-109">Шаг 1. Обзор различий между API</span><span class="sxs-lookup"><span data-stu-id="beedf-109">Step 1: Review the differences between the APIs</span></span>

<span data-ttu-id="beedf-110">Во многих отношениях Microsoft Graph похож на предыдущий Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="beedf-110">In many respects, Microsoft Graph is similar to the earlier Azure AD Graph.</span></span> <span data-ttu-id="beedf-111">Во многих случаях просто измените имя и версию службы конечной точки в коде, и все должно продолжать работать.</span><span class="sxs-lookup"><span data-stu-id="beedf-111">In many cases, simply change the endpoint service name and version in your code, and everything should continue to work.</span></span>

<span data-ttu-id="beedf-112">Тем не менее существуют различия.</span><span class="sxs-lookup"><span data-stu-id="beedf-112">Nonetheless, there are differences.</span></span> <span data-ttu-id="beedf-113">Изменились некоторые ресурсы, свойства, методы и основные возможности.</span><span class="sxs-lookup"><span data-stu-id="beedf-113">Certain resources, properties, methods, and core capabilities have changed.</span></span>

<span data-ttu-id="beedf-114">В частности, и посмотрите на различия в следующих областях:</span><span class="sxs-lookup"><span data-stu-id="beedf-114">Specifically, look for differences in the following areas:</span></span>

- <span data-ttu-id="beedf-115">[Запрос синтаксиса вызовов](migrate-azure-ad-graph-request-differences.md) между двумя службами</span><span class="sxs-lookup"><span data-stu-id="beedf-115">[Request call syntax](migrate-azure-ad-graph-request-differences.md) between the two services</span></span>
- <span data-ttu-id="beedf-116">[Отличия функций,](migrate-azure-ad-graph-feature-differences.md)например расширения каталогов, пакетные пакеты, дифференциальные запросы и так далее</span><span class="sxs-lookup"><span data-stu-id="beedf-116">[Feature differences](migrate-azure-ad-graph-feature-differences.md), such as directory extensions, batching, differential queries, and so on</span></span>
- <span data-ttu-id="beedf-117">[Имена ресурсов Entity и](migrate-azure-ad-graph-resource-differences.md) их типы</span><span class="sxs-lookup"><span data-stu-id="beedf-117">[Entity resource names](migrate-azure-ad-graph-resource-differences.md) and their types</span></span>
- <span data-ttu-id="beedf-118">[Свойства объектов](migrate-azure-ad-graph-property-differences.md) запроса и ответа</span><span class="sxs-lookup"><span data-stu-id="beedf-118">[Properties](migrate-azure-ad-graph-property-differences.md) of request and response objects</span></span>
- <span data-ttu-id="beedf-119">[Методы,](migrate-azure-ad-graph-method-differences.md)включая параметры и типы</span><span class="sxs-lookup"><span data-stu-id="beedf-119">[Methods](migrate-azure-ad-graph-method-differences.md), including parameters and types</span></span>

## <a name="step-2-examine-api-use"></a><span data-ttu-id="beedf-120">Шаг 2. Изучение использования API</span><span class="sxs-lookup"><span data-stu-id="beedf-120">Step 2: Examine API use</span></span>

<span data-ttu-id="beedf-121">[Изучите API,](migrate-azure-ad-graph-audit-api-use.md) используемые вашим приложением, необходимые разрешения и сравните со списком известных различий.</span><span class="sxs-lookup"><span data-stu-id="beedf-121">[Examine the APIs](migrate-azure-ad-graph-audit-api-use.md) used by your app, the permissions they require, and compare to the list of known differences.</span></span>  

<span data-ttu-id="beedf-122">Убедитесь, что API, необходимые вашему приложению, обычно доступны в Microsoft Graph v1.0 и что эти API работают одинаково.</span><span class="sxs-lookup"><span data-stu-id="beedf-122">Verify that the APIs your app needs are generally available in Microsoft Graph v1.0 and that these APIs work the same way.</span></span>

<span data-ttu-id="beedf-123">В некоторых случаях новые возможности и функции предназначены для замены более ранних подходов.</span><span class="sxs-lookup"><span data-stu-id="beedf-123">In some cases, new capabilities and features are designed to replace earlier approaches.</span></span>

<span data-ttu-id="beedf-124">Используйте [обозреватель graph для](https://aka.ms/ge) экспериментов с новыми вызовами и разработки новых подходов.</span><span class="sxs-lookup"><span data-stu-id="beedf-124">Use the [Graph Explorer](https://aka.ms/ge) to experiment with new calls and to develop new approaches.</span></span> <span data-ttu-id="beedf-125">Для наилучших результатов впишитесь с помощью учетных данных тест-пользователя в тестовом клиенте, чтобы увидеть, что API делает над важными наборами данных.</span><span class="sxs-lookup"><span data-stu-id="beedf-125">For best results, sign in using the credentials of a test user in a test tenant so that you see what the API does over important data sets.</span></span>

## <a name="step-3-review-app-details"></a><span data-ttu-id="beedf-126">Шаг 3. Просмотр сведений о приложении</span><span class="sxs-lookup"><span data-stu-id="beedf-126">Step 3: Review app details</span></span>

- <span data-ttu-id="beedf-127">[Изменения регистрации](migrate-azure-ad-graph-app-registration.md) и согласия приложения (которых должно быть нет).</span><span class="sxs-lookup"><span data-stu-id="beedf-127">[App registration](migrate-azure-ad-graph-app-registration.md) and consent changes (which should be none).</span></span>
- <span data-ttu-id="beedf-128">Библиотеки приобретения маркеров [и проверки подлинности.](migrate-azure-ad-graph-authentication-library.md)</span><span class="sxs-lookup"><span data-stu-id="beedf-128">Token acquisition and [authentication libraries](migrate-azure-ad-graph-authentication-library.md).</span></span>
- <span data-ttu-id="beedf-129">Для приложений .NET используйте [клиентские библиотеки.](migrate-azure-ad-graph-client-libraries.md)</span><span class="sxs-lookup"><span data-stu-id="beedf-129">For .NET applications, use of [client libraries](migrate-azure-ad-graph-client-libraries.md).</span></span>

## <a name="step-4-deploy-test-and-extend-your-app"></a><span data-ttu-id="beedf-130">Шаг 4. Развертывание, тестирование и расширение приложения</span><span class="sxs-lookup"><span data-stu-id="beedf-130">Step 4: Deploy, test, and extend your app</span></span>

<span data-ttu-id="beedf-131">Перед обновлением приложения для всех убедитесь, что вы тщательно протестировать и этап вашего выкатки для вашей клиентской аудитории.</span><span class="sxs-lookup"><span data-stu-id="beedf-131">Before updating your app for everyone, ensure you test thoroughly and stage your rollout to your customer audience.</span></span>

<span data-ttu-id="beedf-132">Теперь, когда вы перешли на Microsoft Graph, вам никогда не было проще разблокировать множество наборов данных и функций, которые теперь находятся у вас под рукой.</span><span class="sxs-lookup"><span data-stu-id="beedf-132">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="beedf-133">Вы можете получить вкус того, что возможно, посмотрев на некоторые основные службы и [функции в Microsoft Graph](./overview-major-services.md).</span><span class="sxs-lookup"><span data-stu-id="beedf-133">You can get a taste of what's possible by looking at some of the [Major services and features in Microsoft Graph](./overview-major-services.md).</span></span>

<span data-ttu-id="beedf-134">Если вы в настоящее время используете библиотеку проверки подлинности [ADAL(](/azure/active-directory/develop/active-directory-authentication-libraries) ADAL), рассмотрите возможность перехода на библиотеку проверки подлинности Майкрософт [](/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span><span class="sxs-lookup"><span data-stu-id="beedf-134">If you're currently using the [AD authentication library](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), consider switching to the [Microsoft authentication library](/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span></span>

## <a name="next-steps"></a><span data-ttu-id="beedf-135">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="beedf-135">Next Steps</span></span>

- <span data-ttu-id="beedf-136">Узнайте о [синтаксисе](migrate-azure-ad-graph-request-differences.md) вызовов запросов, чтобы начать шаг 1: рассмотрение различий API.</span><span class="sxs-lookup"><span data-stu-id="beedf-136">Learn about [request call syntax](migrate-azure-ad-graph-request-differences.md) to start step 1: reviewing API differences.</span></span>