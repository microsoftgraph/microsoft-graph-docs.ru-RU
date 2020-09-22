---
title: Общие сведения об API способов проверки подлинности в Azure AD
description: Методы проверки подлинности выполняют проверку подлинности пользователей в Azure AD.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: bb1dd599143447b597c4f57c93b20f3261ecf303
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034124"
---
# <a name="azure-ad-authentication-methods-api-overview"></a><span data-ttu-id="a278c-103">Общие сведения об API способов проверки подлинности в Azure AD</span><span class="sxs-lookup"><span data-stu-id="a278c-103">Azure AD authentication methods API overview</span></span>

<span data-ttu-id="a278c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a278c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a278c-105">[Методы проверки подлинности](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) — это способы проверки подлинности пользователей в Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="a278c-105">[Authentication methods](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods) are the ways that users authenticate in Azure Active Directory (AD).</span></span> <span data-ttu-id="a278c-106">Способы проверки подлинности в Azure AD включают пароль и телефон (например, SMS и голосовые вызовы), которыми можно управлять в Microsoft Graph уже сегодня, и множество других, таких как ключи безопасности FIDO2 и приложение Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="a278c-106">Authentication methods in Azure AD include password and phone (for example, SMS and voice calls), which are manageable in Microsoft Graph today, among many others such as FIDO2 security keys and the Microsoft Authenticator app.</span></span> <span data-ttu-id="a278c-107">Способы проверки подлинности используются в ходе основной, двухфакторной проверки подлинности, проверки подлинности повышенного уровня, а также в процессе самостоятельного сброса пароля (SSPR).</span><span class="sxs-lookup"><span data-stu-id="a278c-107">Authentication methods are used in primary, second-factor, and step-up authentication, and also in the self-service password reset (SSPR) process.</span></span>

<span data-ttu-id="a278c-108">API метода проверки подлинности используются для управления методами проверки подлинности пользователя.</span><span class="sxs-lookup"><span data-stu-id="a278c-108">The authentication method APIs are used to manage a user's authentication methods.</span></span> <span data-ttu-id="a278c-109">Например:</span><span class="sxs-lookup"><span data-stu-id="a278c-109">For example:</span></span>

* <span data-ttu-id="a278c-110">Вы можете добавить номер телефона для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a278c-110">You can add a phone number to a user.</span></span> <span data-ttu-id="a278c-111">После этого пользователь может использовать этот номер телефона для проверки подлинности SMS и голосовых вызовов, если они включены для использования политикой.</span><span class="sxs-lookup"><span data-stu-id="a278c-111">The user can then use that phone number for SMS and voice call authentication if they're enabled to use it by policy.</span></span> 
* <span data-ttu-id="a278c-112">Вы можете обновить этот номер или удалить его из пользователя.</span><span class="sxs-lookup"><span data-stu-id="a278c-112">You can update that number, or delete it from the user.</span></span>
* <span data-ttu-id="a278c-113">Вы можете включить или отключить Ввод номера для входа в SMS.</span><span class="sxs-lookup"><span data-stu-id="a278c-113">You can enable or disable the number for SMS sign-in.</span></span>
* <span data-ttu-id="a278c-114">Вы можете сбросить пароль пользователя.</span><span class="sxs-lookup"><span data-stu-id="a278c-114">You can reset a user's password.</span></span>

## <a name="what-authentication-methods-can-be-managed-in-microsoft-graph"></a><span data-ttu-id="a278c-115">Какие методы проверки подлинности могут управляться в Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="a278c-115">What authentication methods can be managed in Microsoft Graph?</span></span>

|<span data-ttu-id="a278c-116">Способ проверки подлинности </span><span class="sxs-lookup"><span data-stu-id="a278c-116">Authentication method</span></span>       | <span data-ttu-id="a278c-117">Описание</span><span class="sxs-lookup"><span data-stu-id="a278c-117">Description</span></span> |<span data-ttu-id="a278c-118">Примеры</span><span class="sxs-lookup"><span data-stu-id="a278c-118">Examples</span></span>     |
|:---------------------------|:------------|:------------|
|[<span data-ttu-id="a278c-119">пассвордаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="a278c-119">passwordAuthenticationMethod</span></span>](passwordauthenticationmethod.md)| <span data-ttu-id="a278c-120">В настоящее время в Azure AD используется пароль, используемый по умолчанию в качестве основного метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="a278c-120">A password is currently the default primary authentication method in Azure AD.</span></span>|<span data-ttu-id="a278c-121">сбросить пароль пользователя.</span><span class="sxs-lookup"><span data-stu-id="a278c-121">Reset a user's password</span></span>|
|[<span data-ttu-id="a278c-122">фонеаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="a278c-122">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md)|<span data-ttu-id="a278c-123">Пользователь может использовать телефон для проверки подлинности с помощью [SMS или голосовых вызовов](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods#phone-options) (как это разрешено политикой).</span><span class="sxs-lookup"><span data-stu-id="a278c-123">A phone can be used by a user to authenticate using [SMS or voice calls](https://docs.microsoft.com/azure/active-directory/authentication/concept-authentication-methods#phone-options) (as allowed by policy).</span></span>|<span data-ttu-id="a278c-124">Просмотрите номера телефонов проверки подлинности пользователя.</span><span class="sxs-lookup"><span data-stu-id="a278c-124">See a user's authentication phone numbers.</span></span> <span data-ttu-id="a278c-125">Добавление, обновление или удаление номера телефона для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a278c-125">Add, update, or remove a phone number to a user.</span></span> <span data-ttu-id="a278c-126">Включение или отключение основного мобильного телефона для входа в SMS.</span><span class="sxs-lookup"><span data-stu-id="a278c-126">Enable or disable a primary mobile phone for SMS sign-in.</span></span>|

## <a name="next-steps"></a><span data-ttu-id="a278c-127">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="a278c-127">Next steps</span></span>

* <span data-ttu-id="a278c-128">Изучите типы методов проверки подлинности и их различные методы.</span><span class="sxs-lookup"><span data-stu-id="a278c-128">Review the authentication method types and their various methods.</span></span>
* <span data-ttu-id="a278c-129">Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="a278c-129">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>


