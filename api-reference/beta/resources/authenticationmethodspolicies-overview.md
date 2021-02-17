---
title: Обзор API политики методов проверки подлинности Azure AD
description: Политики методов проверки подлинности определяют, какие методы проверки подлинности могут использовать пользователи в Azure AD.
localization_priority: Normal
author: mmcla
ms.author: michmcla
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 593cbea196edcbe1c868a337b1dcfa8a1de2afc9
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271829"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a><span data-ttu-id="658fd-103">Обзор API политик методов проверки подлинности Azure AD</span><span class="sxs-lookup"><span data-stu-id="658fd-103">Azure AD authentication methods policies API overview</span></span>

<span data-ttu-id="658fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="658fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="658fd-105">Политики методов проверки подлинности определяют методы проверки подлинности и пользователей, которые могут использовать их для выполнения многофакторной проверки подлинности (MFA) в Azure Active Directory (Azure AD). [](/azure/active-directory/authentication/concept-authentication-methods)</span><span class="sxs-lookup"><span data-stu-id="658fd-105">Authentication methods policies define [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="658fd-106">Политики методов проверки подлинности, которыми можно управлять в Microsoft Graph, включают ключи безопасности FIDO2 и вход без пароля с помощью приложения Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="658fd-106">Authentication methods policies that can be managed in Microsoft Graph include FIDO2 Security Keys and Passwordless Phone Sign-in with Microsoft Authenticator app.</span></span>

<span data-ttu-id="658fd-107">API политик методов проверки подлинности используются для управления настройками политики.</span><span class="sxs-lookup"><span data-stu-id="658fd-107">The authentication method policies APIs are used to manage policy settings.</span></span> <span data-ttu-id="658fd-108">Например:</span><span class="sxs-lookup"><span data-stu-id="658fd-108">For example:</span></span>

* <span data-ttu-id="658fd-109">Определите типы ключей безопасности FIDO2, которые можно использовать в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="658fd-109">Define the types of FIDO2 security keys that can be used in the Azure AD tenant.</span></span>
* <span data-ttu-id="658fd-110">Определите пользователей или группы пользователей, которым разрешено использовать ключи безопасности FIDO2 или вход в Azure AD без пароля.</span><span class="sxs-lookup"><span data-stu-id="658fd-110">Define the users or groups of users who are allowed to use FIDO2 Security Keys or Passwordless Phone Sign-in to sign in to Azure AD.</span></span>

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a><span data-ttu-id="658fd-111">Какими политиками методов проверки подлинности можно управлять в Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="658fd-111">What authentication methods policies can be managed in Microsoft Graph?</span></span>

|<span data-ttu-id="658fd-112">Политика методов проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="658fd-112">Authentication method policy</span></span>       | <span data-ttu-id="658fd-113">Описание</span><span class="sxs-lookup"><span data-stu-id="658fd-113">Description</span></span> |
|:---------------------------|:------------|:------------|
|[<span data-ttu-id="658fd-114">smsAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="658fd-114">smsAuthenticationMethodConfiguration</span></span>](smsAuthenticationMethodConfiguration.md)| <span data-ttu-id="658fd-115">Определите пользователей, которые могут использовать sms-сообщения в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="658fd-115">Define users who can use Text Message on the Azure AD tenant.</span></span>|
|[<span data-ttu-id="658fd-116">fido2authenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="658fd-116">fido2authenticationmethodconfiguration</span></span>](fido2authenticationmethodconfiguration.md)| <span data-ttu-id="658fd-117">Определите ограничения клавиш безопасности FIDO2 и пользователей, которые могут использовать их для входов в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="658fd-117">Define FIDO2 security key restrictions and users who can use them to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="658fd-118">microsoftauthenticatorauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="658fd-118">microsoftauthenticatorauthenticationmethodconfiguration</span></span>](microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="658fd-119">Определите пользователей, которые могут использовать Microsoft Authenticator в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="658fd-119">Define users who can use Microsoft Authenticator on the Azure AD tenant.</span></span>|
|[<span data-ttu-id="658fd-120">emailauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="658fd-120">emailauthenticationmethodconfiguration</span></span>](emailauthenticationmethodconfiguration.md)|<span data-ttu-id="658fd-121">Определите пользователей, которые могут использовать OTP электронной почты в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="658fd-121">Define users who can use email OTP on the Azure AD tenant.</span></span>|
|<span data-ttu-id="658fd-122">[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (неподдерживаемая)</span><span class="sxs-lookup"><span data-stu-id="658fd-122">[passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md) (deprecated)</span></span>|<span data-ttu-id="658fd-123">Определите пользователей, которые могут использовать для входов в Azure AD телефонный вход без пароля.</span><span class="sxs-lookup"><span data-stu-id="658fd-123">Define users who can use Passwordless Phone Sign-in to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="658fd-124">temporaryaccesspassauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="658fd-124">temporaryaccesspassauthenticationmethodconfiguration</span></span>](temporaryaccesspassauthenticationmethodconfiguration.md)|<span data-ttu-id="658fd-125">Определите пользователей, которые могут использовать временный доступ для входов в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="658fd-125">Define users who can use Temporary Access Pass to sign in to Azure AD.</span></span>|

## <a name="next-steps"></a><span data-ttu-id="658fd-126">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="658fd-126">Next steps</span></span>

* <span data-ttu-id="658fd-127">Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="658fd-127">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
