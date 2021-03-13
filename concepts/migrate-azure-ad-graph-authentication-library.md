---
title: Просмотр изменений библиотеки проверки подлинности приложений
description: Описывает, как обновить использование библиотеки проверки подлинности для переноса приложения из приложений API Azure Active Directory (Azure AD) в API Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: ef49c6a3448dd63a7c933bb40748f218d6fd2db0
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760688"
---
# <a name="review-app-authentication-library-changes"></a><span data-ttu-id="47bba-103">Просмотр изменений библиотеки проверки подлинности приложений</span><span class="sxs-lookup"><span data-stu-id="47bba-103">Review app authentication library changes</span></span>

<span data-ttu-id="47bba-104">Эта статья является *частью шага 3: просмотрите* сведения о процессе переноса [приложений.](migrate-azure-ad-graph-planning-checklist.md)</span><span class="sxs-lookup"><span data-stu-id="47bba-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="47bba-105">Большинство приложений используют библиотеку проверки подлинности для получения и управления маркерами доступа для вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="47bba-105">Most apps use an authentication library to acquire and manage access tokens to call Microsoft Graph.</span></span>  <span data-ttu-id="47bba-106">Корпорация Майкрософт предлагает две библиотеки проверки подлинности:</span><span class="sxs-lookup"><span data-stu-id="47bba-106">Microsoft offers two authentication libraries:</span></span>

- <span data-ttu-id="47bba-107">[Библиотека проверки подлинности Azure Active Directory](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL)</span><span class="sxs-lookup"><span data-stu-id="47bba-107">[Azure Active Directory authentication library](/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL)</span></span>
- <span data-ttu-id="47bba-108">[Библиотека проверки подлинности Майкрософт](/azure/active-directory/develop/reference-v2-libraries) (MSAL)</span><span class="sxs-lookup"><span data-stu-id="47bba-108">[Microsoft authentication library](/azure/active-directory/develop/reference-v2-libraries) (MSAL)</span></span>

## <a name="updating-adal"></a><span data-ttu-id="47bba-109">Обновление ADAL</span><span class="sxs-lookup"><span data-stu-id="47bba-109">Updating ADAL</span></span>

<span data-ttu-id="47bba-110">Если ваше приложение в настоящее время использует ADAL, используйте двух этапный подход к миграции:</span><span class="sxs-lookup"><span data-stu-id="47bba-110">If your app currently uses ADAL, use a two-stage migration approach:</span></span>

1. <span data-ttu-id="47bba-111">Обновите приложение, чтобы получить маркеры доступа для Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="47bba-111">Update your app to acquire access tokens for Microsoft Graph.</span></span> <span data-ttu-id="47bba-112">Продолжайте использовать ADAL для этого шага.</span><span class="sxs-lookup"><span data-stu-id="47bba-112">Continue to use ADAL for this step.</span></span> <span data-ttu-id="47bba-113">Обновление **ресурсаURL,** в котором содержится URI, представляющий веб-API ресурса, из:</span><span class="sxs-lookup"><span data-stu-id="47bba-113">Update the **resourceURL**, which holds the URI representing the resource web API, from:</span></span>

    `https://graph.windows.net`  

    <span data-ttu-id="47bba-114">Кому:</span><span class="sxs-lookup"><span data-stu-id="47bba-114">To:</span></span>  

    `https://graph.microsoft.com`

    <span data-ttu-id="47bba-115">После этого изменения вновь приобретенные маркеры имеют те же области, но аудитория маркеров доступа теперь — Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="47bba-115">Newly acquired tokens have the same scopes after this change, but the audience of the access tokens is now Microsoft Graph.</span></span>  

    <span data-ttu-id="47bba-116">После обновления **resourceURL** и проверки функциональных возможностей выпустите промежуточное обновление, чтобы пользователи могли работать.</span><span class="sxs-lookup"><span data-stu-id="47bba-116">Once you've updated **resourceURL** and verified functionality, release an interim update to get your users up and runnning.</span></span>

1.  <span data-ttu-id="47bba-117">Далее приступить к работе, перенося приложение на использование MSAL, которая является поддерживаемой библиотекой для использования перемещения вперед, теперь, когда ADAL не используется.</span><span class="sxs-lookup"><span data-stu-id="47bba-117">Next, begin work migrating your app to use MSAL, which is the supported library to use moving forward, now that ADAL is deprecated.</span></span>

## <a name="migrating-to-msal"></a><span data-ttu-id="47bba-118">Миграция в MSAL</span><span class="sxs-lookup"><span data-stu-id="47bba-118">Migrating to MSAL</span></span>

<span data-ttu-id="47bba-119">MSAL предоставляет несколько преимуществ над ADAL, в том числе дополнительным согласием, более богатым опытом единой регистрации, поддержкой личных учетных записей Майкрософт, использованием протоколов на основе стандартов и т. д.</span><span class="sxs-lookup"><span data-stu-id="47bba-119">MSAL provides multiple benefits over ADAL, including incremental consent, richer single sign-on experiences, support for personal Microsoft accounts, use of standards-based protocols and so on.</span></span>  

<span data-ttu-id="47bba-120">При переходе приложения на MSAL необходимо внести несколько изменений, в  том числе задав параметр области в запросе на приобретение маркеров:</span><span class="sxs-lookup"><span data-stu-id="47bba-120">When you switch your app over to MSAL, you'll need to make a few changes, including setting the **scopes** parameter in the token acquisition request:</span></span>

``` csharp
var scopes = new string[] { "https://graph.microsoft.com/.default" };
```

<span data-ttu-id="47bba-121">Вышеуказанное выражение ограничивает область разрешений для тех, кто настроен во время регистрации приложений на портале Azure, и сохраняет существующие пользователи от необходимости повторного согласия на ваше приложение.</span><span class="sxs-lookup"><span data-stu-id="47bba-121">The expression above limits the permission scopes request to those configured during application registration in the Azure Portal, and saves your existing users from having to consent to your app again.</span></span>

<span data-ttu-id="47bba-122">См. в справке о переносе [ADAL](https://aka.ms/adal-net-to-msal-net) в MSAL для прямой и обширной помощи в этом процессе, включая устранение неполадок и помощь в устранении распространенных ошибок.</span><span class="sxs-lookup"><span data-stu-id="47bba-122">See [Migrating ADAL to MSAL](https://aka.ms/adal-net-to-msal-net) for direct and extensive help with the process, including troubleshooting and help with common errors.</span></span>

<span data-ttu-id="47bba-123">После миграции в MSAL можно динамически запрашивать дополнительные области, и пользователям будет предложено предоставить дополнительное согласие при следующем использовании приложения.</span><span class="sxs-lookup"><span data-stu-id="47bba-123">Once you've migrated to MSAL, you can request additional scopes dynamically, and users are prompted to provide incremental consent the next time they use your app.</span></span>

## <a name="next-steps"></a><span data-ttu-id="47bba-124">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="47bba-124">Next Steps</span></span>

- <span data-ttu-id="47bba-125">Узнайте о различиях клиентской [библиотеки .NET](migrate-azure-ad-graph-client-libraries.md) между Azure AD Graph и Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="47bba-125">Learn [.NET client library](migrate-azure-ad-graph-client-libraries.md) differences between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="47bba-126">Снова [просмотрите контрольный](migrate-azure-ad-graph-planning-checklist.md) список.</span><span class="sxs-lookup"><span data-stu-id="47bba-126">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>