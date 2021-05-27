---
title: Обзор API политики проверки подлинности Azure AD
description: Политики методов проверки подлинности определяют, какие методы проверки подлинности могут использоваться пользователями в Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 35d3beecb26a5ae4455502ed0535c959cf7f502e
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682133"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a><span data-ttu-id="f1b8a-103">Обзор API политик проверки подлинности Azure AD</span><span class="sxs-lookup"><span data-stu-id="f1b8a-103">Azure AD authentication methods policies API overview</span></span>

<span data-ttu-id="f1b8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1b8a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1b8a-105">Политики методов проверки подлинности определяют методы проверки подлинности и пользователей, которые могут использовать их для регистрации и выполнения многофакторной проверки подлинности (MFA) в Azure Active Directory (Azure AD). [](/azure/active-directory/authentication/concept-authentication-methods)</span><span class="sxs-lookup"><span data-stu-id="f1b8a-105">Authentication methods policies define [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="f1b8a-106">Политики методов проверки подлинности, которыми можно управлять в Microsoft Graph, включают ключи безопасности FIDO2 и Телефон вход с Microsoft Authenticator приложением.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-106">Authentication methods policies that can be managed in Microsoft Graph include FIDO2 Security Keys and Passwordless Phone Sign-in with Microsoft Authenticator app.</span></span>

<span data-ttu-id="f1b8a-107">API-политики методов проверки подлинности используются для управления настройками политики.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-107">The authentication method policies APIs are used to manage policy settings.</span></span> <span data-ttu-id="f1b8a-108">Например:</span><span class="sxs-lookup"><span data-stu-id="f1b8a-108">For example:</span></span>

* <span data-ttu-id="f1b8a-109">Определите типы ключей безопасности FIDO2, которые можно использовать в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-109">Define the types of FIDO2 security keys that can be used in the Azure AD tenant.</span></span>
* <span data-ttu-id="f1b8a-110">Определите пользователей или группы пользователей, которым разрешено использовать ключи безопасности FIDO2 или Телефон для регистрации в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-110">Define the users or groups of users who are allowed to use FIDO2 Security Keys or Passwordless Phone Sign-in to sign in to Azure AD.</span></span>
* <span data-ttu-id="f1b8a-111">Определите пользователей или группы пользователей, которым следует напомнить о Microsoft Authenticator для MFA с помощью push-уведомлений.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-111">Define the users or groups of users who should be reminded to set up the Microsoft Authenticator for MFA using push notifications.</span></span>

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a><span data-ttu-id="f1b8a-112">Какие политики методов проверки подлинности можно управлять в Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="f1b8a-112">What authentication methods policies can be managed in Microsoft Graph?</span></span>

|<span data-ttu-id="f1b8a-113">Политика метода проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="f1b8a-113">Authentication method policy</span></span>       | <span data-ttu-id="f1b8a-114">Описание</span><span class="sxs-lookup"><span data-stu-id="f1b8a-114">Description</span></span> |
|:---------------------------|:------------|
|[<span data-ttu-id="f1b8a-115">smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1b8a-115">smsAuthenticationMethodConfiguration</span></span>](smsAuthenticationMethodConfiguration.md)| <span data-ttu-id="f1b8a-116">Определите пользователей, которые могут использовать текстовое сообщение в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-116">Define users who can use Text Message on the Azure AD tenant.</span></span>|
|[<span data-ttu-id="f1b8a-117">fido2authenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="f1b8a-117">fido2authenticationmethodconfiguration</span></span>](fido2authenticationmethodconfiguration.md)| <span data-ttu-id="f1b8a-118">Определите ограничения ключей безопасности FIDO2 и пользователей, которые могут использовать их для входов в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-118">Define FIDO2 security key restrictions and users who can use them to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="f1b8a-119">microsoftauthenticatorauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="f1b8a-119">microsoftauthenticatorauthenticationmethodconfiguration</span></span>](microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="f1b8a-120">Определите пользователей, которые могут Microsoft Authenticator в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-120">Define users who can use Microsoft Authenticator on the Azure AD tenant.</span></span>|
|[<span data-ttu-id="f1b8a-121">emailauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="f1b8a-121">emailauthenticationmethodconfiguration</span></span>](emailauthenticationmethodconfiguration.md)|<span data-ttu-id="f1b8a-122">Определите пользователей, которые могут использовать OTP электронной почты в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-122">Define users who can use email OTP on the Azure AD tenant.</span></span>|
|<span data-ttu-id="f1b8a-123">[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (deprecated)</span><span class="sxs-lookup"><span data-stu-id="f1b8a-123">[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (deprecated)</span></span>|<span data-ttu-id="f1b8a-124">Определите пользователей, которые могут использовать Телефон для регистрации в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-124">Define users who can use Passwordless Phone Sign-in to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="f1b8a-125">temporaryaccesspassauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="f1b8a-125">temporaryaccesspassauthenticationmethodconfiguration</span></span>](temporaryaccesspassauthenticationmethodconfiguration.md)|<span data-ttu-id="f1b8a-126">Определите пользователей, которые могут использовать временный пропуск доступа для входов в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1b8a-126">Define users who can use Temporary Access Pass to sign in to Azure AD.</span></span>|

## <a name="policies-available-to-push-users-to-set-up-authentication-methods"></a><span data-ttu-id="f1b8a-127">Политики, доступные для того, чтобы подтолкнуть пользователей к настройкам методов проверки подлинности:</span><span class="sxs-lookup"><span data-stu-id="f1b8a-127">Policies available to push users to set up authentication methods:</span></span>
|<span data-ttu-id="f1b8a-128">Политика</span><span class="sxs-lookup"><span data-stu-id="f1b8a-128">Policy</span></span>       | <span data-ttu-id="f1b8a-129">Описание</span><span class="sxs-lookup"><span data-stu-id="f1b8a-129">Description</span></span> |
|:---------------------------|:------------|
|[<span data-ttu-id="f1b8a-130">authenticationMethodsRegistrationCampaign</span><span class="sxs-lookup"><span data-stu-id="f1b8a-130">authenticationMethodsRegistrationCampaign</span></span>](authenticationmethodsregistrationcampaign.md)| <span data-ttu-id="f1b8a-131">Определите пользователей, которым следует напомнить о том, как настроить метод проверки подлинности (поддерживается только для Microsoft Authenticator).</span><span class="sxs-lookup"><span data-stu-id="f1b8a-131">Define users who should be reminded to set up an authentication method (only supported for the Microsoft Authenticator).</span></span>|

## <a name="next-steps"></a><span data-ttu-id="f1b8a-132">Следующие шаги</span><span class="sxs-lookup"><span data-stu-id="f1b8a-132">Next steps</span></span>

* <span data-ttu-id="f1b8a-133">Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="f1b8a-133">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
