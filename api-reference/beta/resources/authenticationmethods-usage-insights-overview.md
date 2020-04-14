---
title: Работа с API отчетов об использовании методов проверки подлинности
description: Отчет об использовании способов проверки подлинности помогает Организации определить, как их конечные пользователи используют функции Azure Active Directory, такие как самостоятельный сброс паролей и многофакторная проверка подлинности (MFA).
localization_priority: Normal
author: kholtz
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: d7f7a8e6cddf308c5681f74ca6546a9467704cc6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472202"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a><span data-ttu-id="1dff0-103">Работа с API отчетов об использовании методов проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="1dff0-103">Working with the authentication methods usage report API</span></span>

<span data-ttu-id="1dff0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dff0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dff0-105">Отчеты об использовании способов проверки подлинности помогают определить, как пользователи в вашей организации используют возможности Azure Active Directory (Azure AD), такие как самостоятельный пароль и многофакторная проверка подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="1dff0-105">The authentication methods usage reports help you understand how users in your organization use Azure Active Directory (Azure AD) capabilities, such as self-service password rest and multi-factor authentication (MFA).</span></span>

<span data-ttu-id="1dff0-106">В этих отчетах представлены следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="1dff0-106">These reports provide information such as:</span></span>

- <span data-ttu-id="1dff0-107">Методы проверки подлинности более успешны для Организации.</span><span class="sxs-lookup"><span data-stu-id="1dff0-107">Which authentication methods are more successful for your organization.</span></span> 
- <span data-ttu-id="1dff0-108">Сведения об ошибках, с которыми работает конечный пользователь.</span><span class="sxs-lookup"><span data-stu-id="1dff0-108">What types of errors end users are running into.</span></span>
- <span data-ttu-id="1dff0-109">Какую кампанию необходимо выполнить, чтобы помочь конечным пользователям принять использование REST пароля и MFA для самостоятельного пароля.</span><span class="sxs-lookup"><span data-stu-id="1dff0-109">What campaign you need to run to help your end users adopt the use of self-service password rest and MFA.</span></span>

## <a name="common-requests"></a><span data-ttu-id="1dff0-110">Общие запросы</span><span class="sxs-lookup"><span data-stu-id="1dff0-110">Common requests</span></span>

<span data-ttu-id="1dff0-111">В следующей таблице перечислены некоторые распространенные запросы, которые можно использовать с этим API.</span><span class="sxs-lookup"><span data-stu-id="1dff0-111">The following table lists some common requests that you can use with this API.</span></span>

| <span data-ttu-id="1dff0-112">Operation</span><span class="sxs-lookup"><span data-stu-id="1dff0-112">Operation</span></span> | <span data-ttu-id="1dff0-113">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="1dff0-113">Try in Graph Explorer</span></span> | <span data-ttu-id="1dff0-114">Описание</span><span class="sxs-lookup"><span data-stu-id="1dff0-114">Description</span></span> |
| --------- | --- | ----------- |
| [<span data-ttu-id="1dff0-115">жеткредентиалусеррегистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="1dff0-115">getCredentialUserRegistrationcount</span></span>](/graph/api/resources/credentialuserregistrationcount?view=graph-rest-beta) | <span data-ttu-id="1dff0-116">[ПОЛУЧЕНИЕ/кредентиалусеррегистратионкаунт](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta)</span><span class="sxs-lookup"><span data-stu-id="1dff0-116">[GET /credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta)</span></span> | <span data-ttu-id="1dff0-117">Получение числа пользователей, зарегистрированных для самостоятельного сброса пароля и MFA.</span><span class="sxs-lookup"><span data-stu-id="1dff0-117">Get the number of users registered for self-service password reset and MFA.</span></span> |
| [<span data-ttu-id="1dff0-118">жеткредентиалусажесуммари</span><span class="sxs-lookup"><span data-stu-id="1dff0-118">getCredentialUsageSummary</span></span>](/graph/api/resources/credentialusagesummary?view=graph-rest-beta) | [<span data-ttu-id="1dff0-119">ПОЛУЧЕНИЕ/кредентиалусажесуммари</span><span class="sxs-lookup"><span data-stu-id="1dff0-119">GET /credentialusagesummary</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | <span data-ttu-id="1dff0-120">Получение числа пользователей, использующих самостоятельный сброс пароля.</span><span class="sxs-lookup"><span data-stu-id="1dff0-120">Get the number of users using self-service password reset.</span></span> |
| [<span data-ttu-id="1dff0-121">кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="1dff0-121">credentialUserRegistrationDetails</span></span>](/graph/api/resources/credentialuserregistrationdetails?view=graph-rest-beta) | [<span data-ttu-id="1dff0-122">ПОЛУЧЕНИЕ/кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="1dff0-122">GET /credentialuserregistrationdetails</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | <span data-ttu-id="1dff0-123">Получение сведений о пользователях для самостоятельного сброса пароля и действий регистрации MFA.</span><span class="sxs-lookup"><span data-stu-id="1dff0-123">Get the user details for self-service password reset and MFA registration activities.</span></span> |
| [<span data-ttu-id="1dff0-124">усеркредентиалусажедетаилс</span><span class="sxs-lookup"><span data-stu-id="1dff0-124">userCredentialUsageDetails</span></span>](/graph/api/resources/usercredentialusagedetails?view=graph-rest-beta) | [<span data-ttu-id="1dff0-125">ПОЛУЧЕНИЕ/усеркредентиалусажедетаилс</span><span class="sxs-lookup"><span data-stu-id="1dff0-125">GET /usercredentialusagedetails</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | <span data-ttu-id="1dff0-126">Получение сведений о пользователях для всех действий самостоятельного сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="1dff0-126">Get user details for all self-service password reset activities.</span></span> |

## <a name="licenses"></a><span data-ttu-id="1dff0-127">Лицензии</span><span class="sxs-lookup"><span data-stu-id="1dff0-127">Licenses</span></span>

<span data-ttu-id="1dff0-128">Отчеты об использовании доступны для лицензионных функций, которые используют преимущества самостоятельного сброса пароля и MFA в клиенте.</span><span class="sxs-lookup"><span data-stu-id="1dff0-128">Usage reports are available for licensed features that take advantage of self-service password reset and MFA in your tenant.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1dff0-129">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1dff0-129">Next steps</span></span>

- <span data-ttu-id="1dff0-130">Сведения о [развертывании средства самообслуживания Azure Active Directory для самостоятельного сброса пароля](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-deployment).</span><span class="sxs-lookup"><span data-stu-id="1dff0-130">Learn how to [deploy Azure Active Directory self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-deployment).</span></span>
- <span data-ttu-id="1dff0-131">Узнайте, как развернуть [Azure Active Directory MFA](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).</span><span class="sxs-lookup"><span data-stu-id="1dff0-131">Learn how to deploy [Azure Active Directory MFA](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).</span></span>
- <span data-ttu-id="1dff0-132">Узнайте, как включить [регистрацию сведений о безопасности в сочетании](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined).</span><span class="sxs-lookup"><span data-stu-id="1dff0-132">Learn how to enable [combined security info registration](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined).</span></span>



