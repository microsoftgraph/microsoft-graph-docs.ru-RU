---
title: Обзор API политики проверки подлинности Azure AD
description: Политики методов проверки подлинности определяют, какие методы проверки подлинности могут использоваться пользователями в Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 5aed8ead61bb9f2dde102dc085e5509945d492f4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964988"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a><span data-ttu-id="7ab45-103">Обзор API политик проверки подлинности Azure AD</span><span class="sxs-lookup"><span data-stu-id="7ab45-103">Azure AD authentication methods policies API overview</span></span>

<span data-ttu-id="7ab45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ab45-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ab45-105">Политики методов проверки подлинности определяют методы проверки подлинности и пользователей, которые могут использовать их для регистрации и выполнения многофакторной проверки подлинности (MFA) в Azure Active Directory (Azure AD). [](/azure/active-directory/authentication/concept-authentication-methods)</span><span class="sxs-lookup"><span data-stu-id="7ab45-105">Authentication methods policies define [authentication methods](/azure/active-directory/authentication/concept-authentication-methods) and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="7ab45-106">Политики методов проверки подлинности, которыми можно управлять в Microsoft Graph, включают ключи безопасности FIDO2 и вход без паролей с помощью приложения Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="7ab45-106">Authentication methods policies that can be managed in Microsoft Graph include FIDO2 Security Keys and Passwordless Phone Sign-in with Microsoft Authenticator app.</span></span>

<span data-ttu-id="7ab45-107">API-политики методов проверки подлинности используются для управления настройками политики.</span><span class="sxs-lookup"><span data-stu-id="7ab45-107">The authentication method policies APIs are used to manage policy settings.</span></span> <span data-ttu-id="7ab45-108">Например:</span><span class="sxs-lookup"><span data-stu-id="7ab45-108">For example:</span></span>

* <span data-ttu-id="7ab45-109">Определите типы ключей безопасности FIDO2, которые можно использовать в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7ab45-109">Define the types of FIDO2 security keys that can be used in the Azure AD tenant.</span></span>
* <span data-ttu-id="7ab45-110">Определите пользователей или группы пользователей, которым разрешено использовать ключи безопасности FIDO2 или вход без паролей для входов в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7ab45-110">Define the users or groups of users who are allowed to use FIDO2 Security Keys or Passwordless Phone Sign-in to sign in to Azure AD.</span></span>

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a><span data-ttu-id="7ab45-111">Какие политики методов проверки подлинности можно управлять в Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="7ab45-111">What authentication methods policies can be managed in Microsoft Graph?</span></span>

|<span data-ttu-id="7ab45-112">Политика метода проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="7ab45-112">Authentication method policy</span></span>       | <span data-ttu-id="7ab45-113">Описание</span><span class="sxs-lookup"><span data-stu-id="7ab45-113">Description</span></span> |
|:---------------------------|:------------|:------------|
|[<span data-ttu-id="7ab45-114">fido2authenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="7ab45-114">fido2authenticationmethodconfiguration</span></span>](fido2authenticationmethodconfiguration.md)| <span data-ttu-id="7ab45-115">Определите ограничения ключей безопасности FIDO2 и пользователей, которые могут использовать их для входов в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7ab45-115">Define FIDO2 security key restrictions and users who can use them to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="7ab45-116">microsoftauthenticatorauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="7ab45-116">microsoftauthenticatorauthenticationmethodconfiguration</span></span>](microsoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="7ab45-117">Определите пользователей, которые могут использовать Microsoft Authenticator в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7ab45-117">Define users who can use Microsoft Authenticator on the Azure AD tenant.</span></span>|
|[<span data-ttu-id="7ab45-118">emailauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="7ab45-118">emailauthenticationmethodconfiguration</span></span>](emailauthenticationmethodconfiguration.md)|<span data-ttu-id="7ab45-119">Определите пользователей, которые могут использовать OTP электронной почты в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7ab45-119">Define users who can use email OTP on the Azure AD tenant.</span></span>|

## <a name="next-steps"></a><span data-ttu-id="7ab45-120">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="7ab45-120">Next steps</span></span>

* <span data-ttu-id="7ab45-121">Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="7ab45-121">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
