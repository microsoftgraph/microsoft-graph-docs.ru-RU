---
title: Контрольный список планирования миграции приложений
description: Контрольный список для переноса приложений из Azure AD Graph в Microsoft Graph
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 84d486cd64d838a00998179a25dbba3ea35738eb
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546933"
---
# <a name="app-migration-planning-checklist"></a><span data-ttu-id="3599d-103">Контрольный список планирования миграции приложений</span><span class="sxs-lookup"><span data-stu-id="3599d-103">App migration planning checklist</span></span>

> [!Important]
> <span data-ttu-id="3599d-104">Теперь Graph API Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3599d-104">Azure AD Graph API is now deprecated.</span></span> <span data-ttu-id="3599d-105">Мы продолжим предоставлять техническую поддержку и обновления для системы безопасности, но больше не будем предоставлять обновления компонентов.</span><span class="sxs-lookup"><span data-stu-id="3599d-105">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
> <span data-ttu-id="3599d-106">Начиная с 30 июня 2022 г., мы переимеем поддержку azure AD Graph и больше не будем предоставлять техническую поддержку или обновления безопасности.</span><span class="sxs-lookup"><span data-stu-id="3599d-106">Starting June 30th, 2022, we will end support for Azure AD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="3599d-107">Приложения с помощью Azure AD Graph после этого времени больше не будут получать ответы из конечной точки Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="3599d-107">Apps using Azure AD Graph after this time will no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="3599d-108">Чтобы спланировать миграцию, используйте следующий контрольный список.</span><span class="sxs-lookup"><span data-stu-id="3599d-108">Use the following checklist to plan your migration.</span></span>

## <a name="step-1-review-the-differences-between-the-apis"></a><span data-ttu-id="3599d-109">Шаг 1. Обзор различий между API</span><span class="sxs-lookup"><span data-stu-id="3599d-109">Step 1: Review the differences between the APIs</span></span>

<span data-ttu-id="3599d-110">Во многих отношениях microsoft Graph аналогично предыдущей платформе Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="3599d-110">In many respects, Microsoft Graph is similar to the earlier Azure AD Graph.</span></span> <span data-ttu-id="3599d-111">Во многих случаях просто измените имя и версию службы конечной точки в коде, и все должно продолжать работать.</span><span class="sxs-lookup"><span data-stu-id="3599d-111">In many cases, simply change the endpoint service name and version in your code, and everything should continue to work.</span></span>

<span data-ttu-id="3599d-112">Тем не менее существуют различия.</span><span class="sxs-lookup"><span data-stu-id="3599d-112">Nonetheless, there are differences.</span></span> <span data-ttu-id="3599d-113">Изменились некоторые ресурсы, свойства, методы и основные возможности.</span><span class="sxs-lookup"><span data-stu-id="3599d-113">Certain resources, properties, methods, and core capabilities have changed.</span></span>

<span data-ttu-id="3599d-114">В частности, и посмотрите на различия в следующих областях:</span><span class="sxs-lookup"><span data-stu-id="3599d-114">Specifically, look for differences in the following areas:</span></span>

- <span data-ttu-id="3599d-115">[Запрос синтаксиса вызовов](migrate-azure-ad-graph-request-differences.md) между двумя службами</span><span class="sxs-lookup"><span data-stu-id="3599d-115">[Request call syntax](migrate-azure-ad-graph-request-differences.md) between the two services</span></span>
- <span data-ttu-id="3599d-116">[Отличия функций,](migrate-azure-ad-graph-feature-differences.md)например расширения каталогов, пакетные пакеты, дифференциальные запросы и так далее</span><span class="sxs-lookup"><span data-stu-id="3599d-116">[Feature differences](migrate-azure-ad-graph-feature-differences.md), such as directory extensions, batching, differential queries, and so on</span></span>
- <span data-ttu-id="3599d-117">[Имена ресурсов Entity и](migrate-azure-ad-graph-resource-differences.md) их типы</span><span class="sxs-lookup"><span data-stu-id="3599d-117">[Entity resource names](migrate-azure-ad-graph-resource-differences.md) and their types</span></span>
- <span data-ttu-id="3599d-118">[Свойства объектов](migrate-azure-ad-graph-property-differences.md) запроса и ответа</span><span class="sxs-lookup"><span data-stu-id="3599d-118">[Properties](migrate-azure-ad-graph-property-differences.md) of request and response objects</span></span>
- <span data-ttu-id="3599d-119">[Методы,](migrate-azure-ad-graph-method-differences.md)включая параметры и типы</span><span class="sxs-lookup"><span data-stu-id="3599d-119">[Methods](migrate-azure-ad-graph-method-differences.md), including parameters and types</span></span>

## <a name="step-2-examine-api-use"></a><span data-ttu-id="3599d-120">Шаг 2. Изучение использования API</span><span class="sxs-lookup"><span data-stu-id="3599d-120">Step 2: Examine API use</span></span>

<span data-ttu-id="3599d-121">[Изучите API,](migrate-azure-ad-graph-audit-api-use.md) используемые вашим приложением, необходимые разрешения и сравните со списком известных различий.</span><span class="sxs-lookup"><span data-stu-id="3599d-121">[Examine the APIs](migrate-azure-ad-graph-audit-api-use.md) used by your app, the permissions they require, and compare to the list of known differences.</span></span>  

<span data-ttu-id="3599d-122">Убедитесь, что API, необходимые вашему приложению, обычно доступны в Microsoft Graph v1.0 и что эти API работают одинаково.</span><span class="sxs-lookup"><span data-stu-id="3599d-122">Verify that the APIs your app needs are generally available in Microsoft Graph v1.0 and that these APIs work the same way.</span></span>

<span data-ttu-id="3599d-123">В некоторых случаях новые возможности и функции предназначены для замены более ранних подходов.</span><span class="sxs-lookup"><span data-stu-id="3599d-123">In some cases, new capabilities and features are designed to replace earlier approaches.</span></span>

<span data-ttu-id="3599d-124">Используйте Graph [Explorer для](https://aka.ms/ge) экспериментов с новыми вызовами и разработки новых подходов.</span><span class="sxs-lookup"><span data-stu-id="3599d-124">Use the [Graph Explorer](https://aka.ms/ge) to experiment with new calls and to develop new approaches.</span></span> <span data-ttu-id="3599d-125">Для наилучших результатов впишитесь с помощью учетных данных тест-пользователя в тестовом клиенте, чтобы увидеть, что API делает над важными наборами данных.</span><span class="sxs-lookup"><span data-stu-id="3599d-125">For best results, sign in using the credentials of a test user in a test tenant so that you see what the API does over important data sets.</span></span>

## <a name="step-3-review-app-details"></a><span data-ttu-id="3599d-126">Шаг 3. Просмотр сведений о приложении</span><span class="sxs-lookup"><span data-stu-id="3599d-126">Step 3: Review app details</span></span>

- <span data-ttu-id="3599d-127">[Изменения регистрации](migrate-azure-ad-graph-app-registration.md) и согласия приложения (которых должно быть нет).</span><span class="sxs-lookup"><span data-stu-id="3599d-127">[App registration](migrate-azure-ad-graph-app-registration.md) and consent changes (which should be none).</span></span>
- <span data-ttu-id="3599d-128">Библиотеки приобретения маркеров [и проверки подлинности.](migrate-azure-ad-graph-authentication-library.md)</span><span class="sxs-lookup"><span data-stu-id="3599d-128">Token acquisition and [authentication libraries](migrate-azure-ad-graph-authentication-library.md).</span></span>
- <span data-ttu-id="3599d-129">Для приложений .NET используйте [клиентские библиотеки.](migrate-azure-ad-graph-client-libraries.md)</span><span class="sxs-lookup"><span data-stu-id="3599d-129">For .NET applications, use of [client libraries](migrate-azure-ad-graph-client-libraries.md).</span></span>

## <a name="step-4-deploy-test-and-extend-your-app"></a><span data-ttu-id="3599d-130">Шаг 4. Развертывание, тестирование и расширение приложения</span><span class="sxs-lookup"><span data-stu-id="3599d-130">Step 4: Deploy, test, and extend your app</span></span>

<span data-ttu-id="3599d-131">Перед обновлением приложения для всех убедитесь, что вы тщательно протестировать и этап вашего выкатки для вашей клиентской аудитории.</span><span class="sxs-lookup"><span data-stu-id="3599d-131">Before updating your app for everyone, ensure you test thoroughly and stage your rollout to your customer audience.</span></span>

<span data-ttu-id="3599d-132">Теперь, когда вы перешли на Microsoft Graph, вам никогда не было проще разблокировать множество наборов данных и функций, которые теперь находятся у вас под рукой.</span><span class="sxs-lookup"><span data-stu-id="3599d-132">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="3599d-133">Вы можете получить вкус того, что возможно, посмотрев на некоторые основные службы и функции в [Microsoft Graph](./overview-major-services.md).</span><span class="sxs-lookup"><span data-stu-id="3599d-133">You can get a taste of what's possible by looking at some of the [Major services and features in Microsoft Graph](./overview-major-services.md).</span></span>

<span data-ttu-id="3599d-134">[Библиотека проверки подлинности](/azure/active-directory/develop/reference-v2-libraries) Майкрософт (MSAL) теперь является рекомендуемой библиотекой проверки подлинности для использования в платформа удостоверений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="3599d-134">[Microsoft authentication library](/azure/active-directory/develop/reference-v2-libraries) (MSAL) is now the recommended authentication library for use with the Microsoft identity platform.</span></span> <span data-ttu-id="3599d-135">Если в настоящее время используется библиотека проверки подлинности [ADAL,](/azure/active-directory/develop/active-directory-authentication-libraries) запланируйте переход на MSAL.</span><span class="sxs-lookup"><span data-stu-id="3599d-135">If you're currently using the [AD authentication library](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), plan to switch to MSAL.</span></span> <span data-ttu-id="3599d-136">Дополнительные рекомендации по переносу приложений в Библиотеку проверки подлинности [Майкрософт (MSAL).](/azure/active-directory/develop/msal-migration)</span><span class="sxs-lookup"><span data-stu-id="3599d-136">See further guidance to [migrate applications to the Microsoft Authentication Library (MSAL)](/azure/active-directory/develop/msal-migration).</span></span>

## <a name="next-steps"></a><span data-ttu-id="3599d-137">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="3599d-137">Next Steps</span></span>

- <span data-ttu-id="3599d-138">Узнайте о [синтаксисе](migrate-azure-ad-graph-request-differences.md) вызовов запросов, чтобы начать шаг 1: рассмотрение различий API.</span><span class="sxs-lookup"><span data-stu-id="3599d-138">Learn about [request call syntax](migrate-azure-ad-graph-request-differences.md) to start step 1: reviewing API differences.</span></span>