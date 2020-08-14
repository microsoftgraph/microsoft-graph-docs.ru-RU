---
title: Обзор API отчетов об удостоверениях и доступе
description: Обращайтесь к отчетам об удостоверениях и доступе, чтобы получить сведения о том, как пользователи в вашей организации используют приложения в клиенте Azure Active Directory.
localization_priority: Priority
ms.prod: microsoft-identity-platform
author: khotz
doc_type: conceptualPageType
ms.openlocfilehash: 140aa4598f643defe42364e99dd0c5a79eb4ab6d
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/14/2020
ms.locfileid: "46673718"
---
# <a name="identity-and-access-reports-api-overview"></a><span data-ttu-id="a81b2-103">Обзор API отчетов об удостоверениях и доступе</span><span class="sxs-lookup"><span data-stu-id="a81b2-103">Identity and access reports API overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a81b2-104">С помощью Microsoft Graph вы можете получать доступ к отчетам об удостоверениях и доступе, чтобы получить сведения о том, как пользователи в вашей организации используют приложения в клиенте Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a81b2-104">With Microsoft Graph, you can use access identity and access reports to get information about how people in your business are using applications in your Azure Active Directory (Azure AD) tenant.</span></span>

## <a name="authorization"></a><span data-ttu-id="a81b2-105">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a81b2-105">Authorization</span></span>

<span data-ttu-id="a81b2-106">Microsoft Graph позволяет управлять доступом к ресурсам, используя разрешения.</span><span class="sxs-lookup"><span data-stu-id="a81b2-106">Microsoft Graph controls access to resources using permissions.</span></span> <span data-ttu-id="a81b2-107">Укажите разрешения, необходимые для доступа к отчетам.</span><span class="sxs-lookup"><span data-stu-id="a81b2-107">You must specify the permissions you need in order to access reports resources.</span></span> <span data-ttu-id="a81b2-108">Дополнительные сведения см. в [справочнике по разрешениям Microsoft Graph](/graph/permissions-reference) и разделе [Разрешения для отчетов](/graph/permissions-reference#reports-permissions).</span><span class="sxs-lookup"><span data-stu-id="a81b2-108">For more information, see [Microsoft Graph permissions reference](/graph/permissions-reference) and [Reports permissions](/graph/permissions-reference#reports-permissions).</span></span>

## <a name="what-are-identity-and-access-reports"></a><span data-ttu-id="a81b2-109">Что такое отчеты об удостоверениях и доступе?</span><span class="sxs-lookup"><span data-stu-id="a81b2-109">What are identity and access reports?</span></span>

<span data-ttu-id="a81b2-110">Указанные ниже отчеты об удостоверениях и доступе позволяют понять работу приложений в клиенте.</span><span class="sxs-lookup"><span data-stu-id="a81b2-110">The following identity and access reports are available to help you understand application activity in your tenant:</span></span>

- <span data-ttu-id="a81b2-111">Активность приложений AD FS</span><span class="sxs-lookup"><span data-stu-id="a81b2-111">AD FS application activity</span></span>
- <span data-ttu-id="a81b2-112">Вход в приложение</span><span class="sxs-lookup"><span data-stu-id="a81b2-112">Application sign-in</span></span>
- <span data-ttu-id="a81b2-113">Регистрация и использование</span><span class="sxs-lookup"><span data-stu-id="a81b2-113">Registration and usage</span></span>

### <a name="ad-fs-application-activity"></a><span data-ttu-id="a81b2-114">Активность приложений AD FS</span><span class="sxs-lookup"><span data-stu-id="a81b2-114">AD FS application activity</span></span>

<span data-ttu-id="a81b2-115">В отчете об активности приложений AD FS содержатся сведения о том, как проверяющая сторона настроена с помощью служб федерации Active Directory (AD FS), обобщенные сведения об использовании, а также о том, можно ли перенести настройку проверяющей стороны в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a81b2-115">The AD FS application activity report provides information about how a relying party is configured with Active Directory Federation Services (AD FS), its aggregated usage, and whether the relying party configuration can be migrated to Azure Active Directory.</span></span> <span data-ttu-id="a81b2-116">Дополнительные сведения см. в ресурсе [relyingPartyDetailedSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="a81b2-116">For more information, see the [relyingPartyDetailedSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta) resource.</span></span>

### <a name="application-sign-in"></a><span data-ttu-id="a81b2-117">Вход в приложение</span><span class="sxs-lookup"><span data-stu-id="a81b2-117">Application sign-in</span></span>

<span data-ttu-id="a81b2-118">Оцените использование входов в приложения в своем клиенте с помощью сводного отчета или отчета, содержащего подробные сведения о входах, такие как количество входов и возникали ли какие-либо ошибки при входе.</span><span class="sxs-lookup"><span data-stu-id="a81b2-118">Evaluate the usage of application sign-ins in your tenant using either a summary report or a report that provides details of sign-ins, such as the number of sign-ins and whether any errors occured during sign-in.</span></span> <span data-ttu-id="a81b2-119">Дополнительные сведения см. в ресурсе [applicationSignInSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="a81b2-119">For more information, see the [applicationSignInSummary](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta) resource.</span></span>

### <a name="registration-and-usage"></a><span data-ttu-id="a81b2-120">Регистрация и использование</span><span class="sxs-lookup"><span data-stu-id="a81b2-120">Registration and usage</span></span>

<span data-ttu-id="a81b2-121">Узнайте подробнее, как пользователи в вашей организации используют функции Azure AD, такие как самостоятельный сброс пароля и многофакторная проверка подлинности (MFA).</span><span class="sxs-lookup"><span data-stu-id="a81b2-121">Get a better understanding of how users in your organization use Azure AD capabilities, such as self-service password rest and multi-factor authentication (MFA).</span></span> <span data-ttu-id="a81b2-122">Вы можете определить, какие методы проверки подлинности более успешны в вашей организации, с какими типами ошибок сталкиваются пользователи и какую кампанию нужно провести, чтобы помочь пользователям с внедрением самостоятельного сброса паролей и MFA.</span><span class="sxs-lookup"><span data-stu-id="a81b2-122">You can determine which authentication methods are more successful for your organization, what types of errors end users are running into, and what campaign you need to run to help your end users adopt the use of self-service password rest and MFA.</span></span> <span data-ttu-id="a81b2-123">Дополнительные сведения см. в статье [API отчетов об использовании методов проверки подлинности](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="a81b2-123">For more information, see the [authentication methods usage report API](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta).</span></span>

## <a name="next-steps"></a><span data-ttu-id="a81b2-124">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="a81b2-124">Next steps</span></span>

<span data-ttu-id="a81b2-125">Ресурсы и API Microsoft Graph открывают новые способы взаимодействия с пользователями и контроля их работы.</span><span class="sxs-lookup"><span data-stu-id="a81b2-125">Reports resources and APIs can open up new ways for you to engage with users and manage their experiences with Microsoft Graph.</span></span> <span data-ttu-id="a81b2-126">Чтобы узнать больше:</span><span class="sxs-lookup"><span data-stu-id="a81b2-126">To learn more:</span></span>

- <span data-ttu-id="a81b2-127">Изучите подробнее методы и свойства ресурсов, наиболее полезных для вашего сценария.</span><span class="sxs-lookup"><span data-stu-id="a81b2-127">Drill down on the methods and properties of the resources most helpful to your scenario.</span></span>
- <span data-ttu-id="a81b2-128">Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="a81b2-128">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
