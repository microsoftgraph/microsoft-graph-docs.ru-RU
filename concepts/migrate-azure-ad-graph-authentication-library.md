---
title: Проверка изменений библиотеки проверки подлинности приложений
description: Описывается обновление использования библиотеки проверки подлинности для переноса приложения из приложений API Azure Active Directory (Azure AD) в API Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 77604945064565f1387553b22a26a0fa871c998d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630267"
---
# <a name="review-app-authentication-library-changes"></a><span data-ttu-id="d5ebb-103">Проверка изменений библиотеки проверки подлинности приложений</span><span class="sxs-lookup"><span data-stu-id="d5ebb-103">Review app authentication library changes</span></span>

<span data-ttu-id="d5ebb-104">Эта статья входит в *Шаг 3: Ознакомьтесь со сведениями о* [процессе миграции приложений](migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="d5ebb-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="d5ebb-105">Большинство приложений используют библиотеку проверки подлинности для акуире и управления маркерами доступа для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d5ebb-105">Most apps use an authentication library to aquire and manage access tokens to call Microsoft Graph.</span></span>  <span data-ttu-id="d5ebb-106">Корпорация Майкрософт предлагает две библиотеки проверки подлинности:</span><span class="sxs-lookup"><span data-stu-id="d5ebb-106">Microsoft offers two authentication libraries:</span></span>

- <span data-ttu-id="d5ebb-107">[Библиотека проверки подлинности Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) ADAL</span><span class="sxs-lookup"><span data-stu-id="d5ebb-107">[Azure Active Directory authentication library](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL)</span></span>
- <span data-ttu-id="d5ebb-108">[Библиотека проверки](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) подлинности (Майкрософт) MSAL</span><span class="sxs-lookup"><span data-stu-id="d5ebb-108">[Microsoft authentication library](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) (MSAL)</span></span>

## <a name="updating-adal"></a><span data-ttu-id="d5ebb-109">Обновление ADAL</span><span class="sxs-lookup"><span data-stu-id="d5ebb-109">Updating ADAL</span></span>

<span data-ttu-id="d5ebb-110">Если ваше приложение использует ADAL, используйте подход к миграции на два этапа:</span><span class="sxs-lookup"><span data-stu-id="d5ebb-110">If your app currently uses ADAL, use a two-stage migration approach:</span></span>

1. <span data-ttu-id="d5ebb-111">Обновите приложение, чтобы получить маркеры доступа для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d5ebb-111">Update your app to acquire access tokens for Microsoft Graph.</span></span> <span data-ttu-id="d5ebb-112">Продолжайте использовать ADAL для этого этапа.</span><span class="sxs-lookup"><span data-stu-id="d5ebb-112">Continue to use ADAL for this step.</span></span> <span data-ttu-id="d5ebb-113">Обновите **resourceurl экземпляром**, который содержит URI, представляющий веб-API ресурсов, от:</span><span class="sxs-lookup"><span data-stu-id="d5ebb-113">Update the **resourceURL**, which holds the URI representing the resource web API, from:</span></span>

    `https://graph.windows.net`  

    <span data-ttu-id="d5ebb-114">Кому:</span><span class="sxs-lookup"><span data-stu-id="d5ebb-114">To:</span></span>  

    `https://graph.microsoft.com`

    <span data-ttu-id="d5ebb-115">Новые приобретенные маркеры имеют те же области после этого изменения, но аудитория маркеров доступа теперь называется Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d5ebb-115">Newly acquired tokens have the same scopes after this change, but the audience of the access tokens is now Microsoft Graph.</span></span>  

    <span data-ttu-id="d5ebb-116">После обновления **resourceurl экземпляром** и проверки работоспособности выпустите промежуточное обновление, чтобы получить доступ к пользователям и рунннинг.</span><span class="sxs-lookup"><span data-stu-id="d5ebb-116">Once you've updated **resourceURL** and verified functionality, release an interim update to get your users up and runnning.</span></span>

1.  <span data-ttu-id="d5ebb-117">Затем начните работу с переносом приложения, чтобы использовать MSAL, поддерживаемую библиотекой, чтобы использовать перемещение вперед.</span><span class="sxs-lookup"><span data-stu-id="d5ebb-117">Next, begin work migrating your app to use MSAL, which is the supported library to use moving forward.</span></span>

## <a name="migrating-to-msal"></a><span data-ttu-id="d5ebb-118">Миграция в MSAL</span><span class="sxs-lookup"><span data-stu-id="d5ebb-118">Migrating to MSAL</span></span>

<span data-ttu-id="d5ebb-119">MSAL предоставляет несколько преимуществ по сравнению с ADAL, в том числе последовательное разрешение, более широкие возможности единого входа, поддержку личных учетных записей Майкрософт, использование протоколов на основе стандартов и т. д.</span><span class="sxs-lookup"><span data-stu-id="d5ebb-119">MSAL provides multiple benefits over ADAL, including incremental consent, richer single sign-on experiences, support for personal Microsoft accounts, use of standards-based protocols and so on.</span></span>  

<span data-ttu-id="d5ebb-120">При переключении приложения на MSAL необходимо внести несколько изменений, в том числе задать параметр Scopes в запросе аккуистион \*\*\*\* маркеров:</span><span class="sxs-lookup"><span data-stu-id="d5ebb-120">When you switch your app over to MSAL, you'll need to make a few changes, including setting the **scopes** parameter in the token acquistion request:</span></span>

``` csharp
var scopes = new string[] { "https://graph.microsoft.com/.default" };
```

<span data-ttu-id="d5ebb-121">Выражение выше ограничивает область разрешений запросами, настроенными во время регистрации приложения на портале Azure, и сохраняет существующих пользователей от необходимости подтверждения приложения.</span><span class="sxs-lookup"><span data-stu-id="d5ebb-121">The expression above limits the permission scopes request to those configured during application registration in the Azure Portal, and saves your existing users from having to consent to your app again.</span></span>

<span data-ttu-id="d5ebb-122">В статье [Миграция ADAL в MSAL](https://aka.ms/adal-net-to-msal-net) для непосредственной и обширной справки по процессу, включая устранение неполадок и справку по распространенным ошибкам.</span><span class="sxs-lookup"><span data-stu-id="d5ebb-122">See [Migrating ADAL to MSAL](https://aka.ms/adal-net-to-msal-net) for direct and extensive help with the process, including troubleshooting and help with common errors.</span></span>

<span data-ttu-id="d5ebb-123">После переноса в MSAL вы можете динамически запрашивать дополнительные области, а пользователям будет предложено получить добавочное согласие при следующем использовании приложения.</span><span class="sxs-lookup"><span data-stu-id="d5ebb-123">Once you've migrated to MSAL, you can request additional scopes dynamically, and users are prompted to provide incremental consent the next time they use your app.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d5ebb-124">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="d5ebb-124">Next Steps</span></span>

- <span data-ttu-id="d5ebb-125">Ознакомьтесь с различиями в [клиентской библиотеке .NET](migrate-azure-ad-graph-client-libraries.md) между Azure AD Graph и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d5ebb-125">Learn [.NET client library](migrate-azure-ad-graph-client-libraries.md) differences between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="d5ebb-126">Изучите [Перенос ADAL в MSAL](https://aka.ms/adal-net-to-msal-net) для получения дополнительной справки по переходу на MSAL.</span><span class="sxs-lookup"><span data-stu-id="d5ebb-126">Explore [Migrating ADAL to MSAL](https://aka.ms/adal-net-to-msal-net) for more in-depth help on migrating to MSAL.</span></span>
- <span data-ttu-id="d5ebb-127">Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .</span><span class="sxs-lookup"><span data-stu-id="d5ebb-127">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="d5ebb-128">Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .</span><span class="sxs-lookup"><span data-stu-id="d5ebb-128">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
