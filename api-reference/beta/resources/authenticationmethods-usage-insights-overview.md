---
title: Работа с API отчетов об использовании методов проверки подлинности
description: Отчет об использовании способов проверки подлинности помогает Организации определить, как их конечные пользователи используют функции Azure Active Directory, такие как самостоятельный сброс паролей и многофакторная проверка подлинности (MFA).
author: davidmu1
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 19f99b0909a762201ea91399125bba841d705338
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35505507"
---
# <a name="working-with-the-authentication-methods-usage-report-api"></a><span data-ttu-id="005ed-103">Работа с API отчетов об использовании методов проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="005ed-103">Working with the authentication methods usage report API</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="005ed-104">Отчеты об использовании способов проверки подлинности помогают определить, как пользователи в вашей организации используют возможности Azure Active Directory (Azure AD), такие как самостоятельный пароль и многофакторная проверка подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="005ed-104">The authentication methods usage reports help you understand how users in your organization use Azure Active Directory (Azure AD) capabilities, such as self-service password rest and multi-factor authentication (MFA).</span></span>

<span data-ttu-id="005ed-105">В этих отчетах представлены следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="005ed-105">These reports provide information such as:</span></span>

- <span data-ttu-id="005ed-106">Методы проверки подлинности более успешны для Организации.</span><span class="sxs-lookup"><span data-stu-id="005ed-106">Which authentication methods are more successful for your organization.</span></span> 
- <span data-ttu-id="005ed-107">Сведения об ошибках, с которыми работает конечный пользователь.</span><span class="sxs-lookup"><span data-stu-id="005ed-107">What types of errors end users are running into.</span></span>
- <span data-ttu-id="005ed-108">Какую кампанию необходимо выполнить, чтобы помочь конечным пользователям принять использование REST пароля и MFA для самостоятельного пароля.</span><span class="sxs-lookup"><span data-stu-id="005ed-108">What campaign you need to run to help your end users adopt the use of self-service password rest and MFA.</span></span>

## <a name="common-requests"></a><span data-ttu-id="005ed-109">Общие запросы</span><span class="sxs-lookup"><span data-stu-id="005ed-109">Common requests</span></span>

<span data-ttu-id="005ed-110">В следующей таблице перечислены некоторые распространенные запросы, которые можно использовать с этим API.</span><span class="sxs-lookup"><span data-stu-id="005ed-110">The following table lists some common requests that you can use with this API.</span></span>

| <span data-ttu-id="005ed-111">Operation</span><span class="sxs-lookup"><span data-stu-id="005ed-111">Operation</span></span> | <span data-ttu-id="005ed-112">Попробовать в песочнице Graph</span><span class="sxs-lookup"><span data-stu-id="005ed-112">Try in Graph Explorer</span></span> | <span data-ttu-id="005ed-113">Описание</span><span class="sxs-lookup"><span data-stu-id="005ed-113">Description</span></span> |
| --------- | --- | ----------- |
| [<span data-ttu-id="005ed-114">Жеткредентиалусеррегистратионкаунт</span><span class="sxs-lookup"><span data-stu-id="005ed-114">getCredentialUserRegistrationcount</span></span>](/graph/api/resources/credentialUserRegistrationCount?view=graph-rest-beta) | <span data-ttu-id="005ed-115">[ПОЛУЧЕНИЕ/кредентиалусеррегистратионкаунт](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta)</span><span class="sxs-lookup"><span data-stu-id="005ed-115">[GET /credentialuserregistrationcount](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUserRegistrationcount()&version=beta)</span></span> | <span data-ttu-id="005ed-116">Получение числа пользователей, зарегистрированных для самостоятельного сброса пароля и MFA.</span><span class="sxs-lookup"><span data-stu-id="005ed-116">Get the number of users registered for self-service password reset and MFA.</span></span> |
| [<span data-ttu-id="005ed-117">Жеткредентиалусажесуммари</span><span class="sxs-lookup"><span data-stu-id="005ed-117">getCredentialUsageSummary</span></span>](/graph/api/resources/credentialUsagesSummary?view=graph-rest-beta) | [<span data-ttu-id="005ed-118">ПОЛУЧЕНИЕ/кредентиалусажесуммари</span><span class="sxs-lookup"><span data-stu-id="005ed-118">GET /credentialusagesummary</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/getCredentialUsageSummary&version=beta) | <span data-ttu-id="005ed-119">Получение числа пользователей, использующих самостоятельный сброс пароля.</span><span class="sxs-lookup"><span data-stu-id="005ed-119">Get the number of users using self-service password reset.</span></span> |
| [<span data-ttu-id="005ed-120">Кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="005ed-120">credentialUserRegistrationDetails</span></span>](/graph/api/resources/credentialUserRegistrationDetails?view=graph-rest-beta) | [<span data-ttu-id="005ed-121">ПОЛУЧЕНИЕ/кредентиалусеррегистратиондетаилс</span><span class="sxs-lookup"><span data-stu-id="005ed-121">GET /credentialuserregistrationdetails</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/credentialUserRegistrationDetails&version=beta) | <span data-ttu-id="005ed-122">Получение сведений о пользователях для самостоятельного сброса пароля и действий регистрации MFA.</span><span class="sxs-lookup"><span data-stu-id="005ed-122">Get the user details for self-service password reset and MFA registration activities.</span></span> |
| [<span data-ttu-id="005ed-123">Усеркредентиалусажедетаилс</span><span class="sxs-lookup"><span data-stu-id="005ed-123">userCredentialUsageDetails</span></span>](/graph/api/resources/userCredentialUsageDetails?view=graph-rest-beta) | [<span data-ttu-id="005ed-124">ПОЛУЧЕНИЕ/усеркредентиалусажедетаилс</span><span class="sxs-lookup"><span data-stu-id="005ed-124">GET /usercredentialusagedetails</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=reports/userCredentialUsageDetails&version=beta) | <span data-ttu-id="005ed-125">Получение сведений о пользователях для всех действий самостоятельного сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="005ed-125">Get user details for all self-service password reset activities.</span></span> |

## <a name="licenses"></a><span data-ttu-id="005ed-126">Лицензии</span><span class="sxs-lookup"><span data-stu-id="005ed-126">Licenses</span></span>

<span data-ttu-id="005ed-127">Отчеты об использовании доступны для лицензионных функций, которые используют преимущества самостоятельного сброса пароля и MFA в клиенте.</span><span class="sxs-lookup"><span data-stu-id="005ed-127">Usage reports are available for licensed features that take advantage of self-service password reset and MFA in your tenant.</span></span>

## <a name="next-steps"></a><span data-ttu-id="005ed-128">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="005ed-128">Next steps</span></span>

- <span data-ttu-id="005ed-129">Сведения о [развертывании средства самообслуживания Azure Active Directory для самостоятельного сброса пароля](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-deployment).</span><span class="sxs-lookup"><span data-stu-id="005ed-129">Learn how to [deploy Azure Active Directory self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-deployment).</span></span>
- <span data-ttu-id="005ed-130">Узнайте, как развернуть [Azure Active Directory MFA](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).</span><span class="sxs-lookup"><span data-stu-id="005ed-130">Learn how to deploy [Azure Active Directory MFA](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).</span></span>
- <span data-ttu-id="005ed-131">Узнайте, как включить [регистрацию сведений о безопасности в сочетании](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined).</span><span class="sxs-lookup"><span data-stu-id="005ed-131">Learn how to enable [combined security info registration](https://docs.microsoft.com/azure/active-directory/authentication/howto-registration-mfa-sspr-combined).</span></span>



