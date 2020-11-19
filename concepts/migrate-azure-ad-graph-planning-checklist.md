---
title: Контрольный список планирования миграции приложений
description: Контрольный список для переноса приложений из Azure AD Graph в Microsoft Graph
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: d6a5fc83717c2facbbb016cbbc621d6d1bb36dc0
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352405"
---
# <a name="app-migration-planning-checklist"></a><span data-ttu-id="de488-103">Контрольный список планирования миграции приложений</span><span class="sxs-lookup"><span data-stu-id="de488-103">App migration planning checklist</span></span>

> [!Important]
> <span data-ttu-id="de488-104">API Graph Azure AD теперь устарел.</span><span class="sxs-lookup"><span data-stu-id="de488-104">Azure AD Graph API is now deprecated.</span></span> <span data-ttu-id="de488-105">Мы будем продолжать предоставлять техническую поддержку и обновления для системы безопасности, но не будут предоставлять обновления компонентов.</span><span class="sxs-lookup"><span data-stu-id="de488-105">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
> <span data-ttu-id="de488-106">Начиная с 30 июня 2022 г. мы завершаем поддержку Azure AD Graph и больше не будут предоставлять техническую поддержку или обновления для системы безопасности.</span><span class="sxs-lookup"><span data-stu-id="de488-106">Starting June 30th, 2022, we will end support for Azure AD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="de488-107">Приложения, использующие Azure AD Graph после этого, больше не будут получать ответы от конечной точки Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="de488-107">Apps using Azure AD Graph after this time will no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="de488-108">Используйте следующий контрольный список для планирования миграции.</span><span class="sxs-lookup"><span data-stu-id="de488-108">Use the following checklist to plan your migration.</span></span>

## <a name="step-1-review-the-differences-between-the-apis"></a><span data-ttu-id="de488-109">Шаг 1: Ознакомьтесь с различиями между API</span><span class="sxs-lookup"><span data-stu-id="de488-109">Step 1: Review the differences between the APIs</span></span>

<span data-ttu-id="de488-110">Во многих отношениях Microsoft Graph аналогичен более ранней версии Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="de488-110">In many respects, Microsoft Graph is similar to the earlier Azure AD Graph.</span></span> <span data-ttu-id="de488-111">Во многих случаях просто измените имя и версию службы конечных точек в коде, и все должно продолжать работу.</span><span class="sxs-lookup"><span data-stu-id="de488-111">In many cases, simply change the endpoint service name and version in your code, and everything should continue to work.</span></span>

<span data-ttu-id="de488-112">Тем не менее, существуют различия.</span><span class="sxs-lookup"><span data-stu-id="de488-112">Nonetheless, there are differences.</span></span> <span data-ttu-id="de488-113">Изменены некоторые ресурсы, свойства, методы и основные возможности.</span><span class="sxs-lookup"><span data-stu-id="de488-113">Certain resources, properties, methods, and core capabilities have changed.</span></span>

<span data-ttu-id="de488-114">В частности, ищите различия в следующих областях:</span><span class="sxs-lookup"><span data-stu-id="de488-114">Specifically, look for differences in the following areas:</span></span>

- <span data-ttu-id="de488-115">[Синтаксис запроса на вызов](migrate-azure-ad-graph-request-differences.md) между двумя службами</span><span class="sxs-lookup"><span data-stu-id="de488-115">[Request call syntax](migrate-azure-ad-graph-request-differences.md) between the two services</span></span>
- <span data-ttu-id="de488-116">[Различия в функциях](migrate-azure-ad-graph-feature-differences.md), такие как расширения каталогов, пакетная обработка, разностные запросы и т. д.</span><span class="sxs-lookup"><span data-stu-id="de488-116">[Feature differences](migrate-azure-ad-graph-feature-differences.md), such as directory extensions, batching, differential queries, and so on</span></span>
- <span data-ttu-id="de488-117">[Имена ресурсов сущностей](migrate-azure-ad-graph-resource-differences.md) и их типы</span><span class="sxs-lookup"><span data-stu-id="de488-117">[Entity resource names](migrate-azure-ad-graph-resource-differences.md) and their types</span></span>
- <span data-ttu-id="de488-118">[Свойства](migrate-azure-ad-graph-property-differences.md) объектов Request и Response</span><span class="sxs-lookup"><span data-stu-id="de488-118">[Properties](migrate-azure-ad-graph-property-differences.md) of request and response objects</span></span>
- <span data-ttu-id="de488-119">[Методы](migrate-azure-ad-graph-method-differences.md), включая параметры и типы</span><span class="sxs-lookup"><span data-stu-id="de488-119">[Methods](migrate-azure-ad-graph-method-differences.md), including parameters and types</span></span>

## <a name="step-2-examine-api-use"></a><span data-ttu-id="de488-120">Шаг 2: Проверка использования API</span><span class="sxs-lookup"><span data-stu-id="de488-120">Step 2: Examine API use</span></span>

<span data-ttu-id="de488-121">[Изучите API](migrate-azure-ad-graph-audit-api-use.md) , используемые вашим приложением, необходимые разрешения и сравните со списком известных отличий.</span><span class="sxs-lookup"><span data-stu-id="de488-121">[Examine the APIs](migrate-azure-ad-graph-audit-api-use.md) used by your app, the permissions they require, and compare to the list of known differences.</span></span>  

<span data-ttu-id="de488-122">Убедитесь, что нужные API-интерфейсы, как правило, доступны в Microsoft Graph версии 1.0, и что эти API работают одинаковым образом.</span><span class="sxs-lookup"><span data-stu-id="de488-122">Verify that the APIs your app needs are generally available in Microsoft Graph v1.0 and that these APIs work the same way.</span></span>

<span data-ttu-id="de488-123">В некоторых случаях новые возможности и функции предназначены для замены более ранних подходов.</span><span class="sxs-lookup"><span data-stu-id="de488-123">In some cases, new capabilities and features are designed to replace earlier approaches.</span></span>

<span data-ttu-id="de488-124">Используйте [проводник Graph](https://aka.ms/ge) для экспериментов с новыми вызовами и разработки новых подходов.</span><span class="sxs-lookup"><span data-stu-id="de488-124">Use the [Graph Explorer](https://aka.ms/ge) to experiment with new calls and to develop new approaches.</span></span> <span data-ttu-id="de488-125">Для достижения лучших результатов Войдите в систему, используя учетные данные тестового пользователя в тестовом клиенте, чтобы увидеть, что API выполняет над важными наборами данных.</span><span class="sxs-lookup"><span data-stu-id="de488-125">For best results, sign in using the credentials of a test user in a test tenant so that you see what the API does over important data sets.</span></span>

## <a name="step-3-review-app-details"></a><span data-ttu-id="de488-126">Шаг 3: Просмотр сведений о приложении</span><span class="sxs-lookup"><span data-stu-id="de488-126">Step 3: Review app details</span></span>

- <span data-ttu-id="de488-127">Изменения регистрации и согласия [приложения](migrate-azure-ad-graph-app-registration.md) (не должно быть None).</span><span class="sxs-lookup"><span data-stu-id="de488-127">[App registration](migrate-azure-ad-graph-app-registration.md) and consent changes (which should be none).</span></span>
- <span data-ttu-id="de488-128">Получение маркеров и [библиотек проверки подлинности](migrate-azure-ad-graph-authentication-library.md).</span><span class="sxs-lookup"><span data-stu-id="de488-128">Token acquisition and [authentication libraries](migrate-azure-ad-graph-authentication-library.md).</span></span>
- <span data-ttu-id="de488-129">Для приложений .NET используйте [клиентские библиотеки](migrate-azure-ad-graph-client-libraries.md).</span><span class="sxs-lookup"><span data-stu-id="de488-129">For .NET applications, use of [client libraries](migrate-azure-ad-graph-client-libraries.md).</span></span>

## <a name="step-4-deploy-test-and-extend-your-app"></a><span data-ttu-id="de488-130">Шаг 4: развертывание, тестирование и расширение приложения</span><span class="sxs-lookup"><span data-stu-id="de488-130">Step 4: Deploy, test, and extend your app</span></span>

<span data-ttu-id="de488-131">Прежде чем обновлять приложение для всех пользователей, убедитесь, что вы тщательно протестируете и разработайте перед развертыванием вашей аудитории клиентов.</span><span class="sxs-lookup"><span data-stu-id="de488-131">Before updating your app for everyone, ensure you test thoroughly and stage your rollout to your customer audience.</span></span>

<span data-ttu-id="de488-132">Теперь, когда вы переключились на Microsoft Graph, вы не сможете упростить разблокировку многих дополнительных наборов данных и функций, которые теперь доступны вам.</span><span class="sxs-lookup"><span data-stu-id="de488-132">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="de488-133">Вы можете получить сведения о возможных возможностях, изучив некоторые [основные службы и функции Microsoft Graph](/graph/overview-major-services).</span><span class="sxs-lookup"><span data-stu-id="de488-133">You can get a taste of what's possible by looking at some of the [Major services and features in Microsoft Graph](/graph/overview-major-services).</span></span>

<span data-ttu-id="de488-134">Если вы используете [библиотеку проверки подлинности Active Directory](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), рассмотрите возможность переключения на [библиотеку проверки подлинности Microsoft](/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span><span class="sxs-lookup"><span data-stu-id="de488-134">If you're currently using the [AD authentication library](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL), consider switching to the [Microsoft authentication library](/azure/active-directory/develop/reference-v2-libraries) (MSAL).</span></span>

## <a name="next-steps"></a><span data-ttu-id="de488-135">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="de488-135">Next Steps</span></span>

- <span data-ttu-id="de488-136">Сведения о [синтаксисе запроса request](migrate-azure-ad-graph-request-differences.md) для начала действия 1: обзор различий API.</span><span class="sxs-lookup"><span data-stu-id="de488-136">Learn about [request call syntax](migrate-azure-ad-graph-request-differences.md) to start step 1: reviewing API differences.</span></span>