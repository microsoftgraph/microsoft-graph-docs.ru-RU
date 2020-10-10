---
title: Общие сведения об API политики проверки подлинности в Azure AD
description: Методы проверки подлинности политики определяют, какие методы проверки подлинности могут использоваться пользователями в Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 1a4c5c94999885ba01112f6f18bea96e93a5e77b
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418479"
---
# <a name="azure-ad-authentication-methods-policies-api-overview"></a><span data-ttu-id="b2646-103">Общие сведения о политиках методов проверки подлинности в Azure AD</span><span class="sxs-lookup"><span data-stu-id="b2646-103">Azure AD authentication methods policies API overview</span></span>

<span data-ttu-id="b2646-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2646-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2646-105">Методы проверки подлинности политики определяют [методы проверки подлинности](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) и пользователей, которым разрешено использовать их для входа и выполнения многофакторной проверки подлинности (MFA) в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="b2646-105">Authentication methods policies define [authentication methods](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) and the users that are allowed to use them to sign in and perform multi-factor authentication (MFA) in Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="b2646-106">Методы проверки подлинности, которые могут управляться в Microsoft Graph, включают ключи безопасности FIDO2 и мобильный вход с помощью приложения Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="b2646-106">Authentication methods policies that can be managed in Microsoft Graph include FIDO2 Security Keys and Passwordless Phone Sign-in with Microsoft Authenticator app.</span></span>

<span data-ttu-id="b2646-107">Для управления параметрами политики используются API политик метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="b2646-107">The authentication method policies APIs are used to manage policy settings.</span></span> <span data-ttu-id="b2646-108">Например,</span><span class="sxs-lookup"><span data-stu-id="b2646-108">For example:</span></span>

* <span data-ttu-id="b2646-109">Определите типы ключей безопасности FIDO2, которые можно использовать в клиенте Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b2646-109">Define the types of FIDO2 security keys that can be used in the Azure AD tenant.</span></span>
* <span data-ttu-id="b2646-110">Определите пользователей или группы пользователей, которым разрешено использовать ключи безопасности FIDO2 или вход без пароля, чтобы войти в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b2646-110">Define the users or groups of users who are allowed to use FIDO2 Security Keys or Passwordless Phone Sign-in to sign in to Azure AD.</span></span>

## <a name="what-authentication-methods-policies-can-be-managed-in-microsoft-graph"></a><span data-ttu-id="b2646-111">Какие политики способов проверки подлинности могут управляться в Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="b2646-111">What authentication methods policies can be managed in Microsoft Graph?</span></span>

|<span data-ttu-id="b2646-112">Политика метода проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b2646-112">Authentication method policy</span></span>       | <span data-ttu-id="b2646-113">Описание</span><span class="sxs-lookup"><span data-stu-id="b2646-113">Description</span></span> |
|:---------------------------|:------------|:------------|
|[<span data-ttu-id="b2646-114">fido2authenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="b2646-114">fido2authenticationmethodconfiguration</span></span>](fido2authenticationmethodconfiguration.md)| <span data-ttu-id="b2646-115">Определите ограничения ключа безопасности FIDO2 и пользователей, которые могут использовать их для входа в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b2646-115">Define FIDO2 security key restrictions and users who can use them to sign in to Azure AD.</span></span>|
|[<span data-ttu-id="b2646-116">пассвордлессмикрософтаусентикатораусентикатионмесодконфигуратион</span><span class="sxs-lookup"><span data-stu-id="b2646-116">passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration</span></span>](passwordlessmicrosoftauthenticatorauthenticationmethodconfiguration.md)|<span data-ttu-id="b2646-117">Определите пользователей, которые могут использовать вход без пароля, чтобы войти в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b2646-117">Define users who can use Passwordless Phone Sign-in to sign in to Azure AD.</span></span>|

## <a name="next-steps"></a><span data-ttu-id="b2646-118">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b2646-118">Next steps</span></span>

* <span data-ttu-id="b2646-119">Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="b2646-119">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
