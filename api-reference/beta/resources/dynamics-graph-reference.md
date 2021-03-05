---
title: Работа с центральным API Dynamics 365 в Microsoft Graph
description: Документация по API для интеграции с Microsoft Graph
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: conceptualPageType
ms.openlocfilehash: b1fdc91d884c4c0869b97f2068d005407158d6a5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473590"
---
# <a name="working-with-the-dynamics-365-business-central-api-in-microsoft-graph"></a><span data-ttu-id="504f7-103">Работа с центральным API Dynamics 365 в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="504f7-103">Working with the Dynamics 365 Business Central API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="504f7-104">Вы можете использовать Microsoft Graph для подключения и интеграции веб-службы или решения SaaS с Microsoft Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="504f7-104">You can use Microsoft Graph to connect and integrate your web service or SaaS solution with Microsoft Dynamics 365 Business Central.</span></span> <span data-ttu-id="504f7-105">С помощью Microsoft Graph можно создавать приложения, которые получают авторизованный доступ к данным Microsoft Dynamics 365 Business Central и интегрируются с ними без проблем.</span><span class="sxs-lookup"><span data-stu-id="504f7-105">With Microsoft Graph, you can build apps that get authorized access to and integrate seamlessly with Microsoft Dynamics 365 Business Central data.</span></span>

## <a name="authorization"></a><span data-ttu-id="504f7-106">Авторизация</span><span class="sxs-lookup"><span data-stu-id="504f7-106">Authorization</span></span>
<span data-ttu-id="504f7-107">Используйте конечную точку Azure AD v2.0 для проверки подлинности API Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="504f7-107">Use the Azure AD v2.0 endpoint to authenticate Dynamics 365 Business Central APIs.</span></span> <span data-ttu-id="504f7-108">Все API требуют `Authorization: Bearer {access-token}` загона запроса.</span><span class="sxs-lookup"><span data-stu-id="504f7-108">All APIs require the `Authorization: Bearer {access-token}` request header.</span></span> <span data-ttu-id="504f7-109">Дополнительные сведения о авторизации см. в записи [Get access tokens to call Microsoft Graph.](/graph/auth/)</span><span class="sxs-lookup"><span data-stu-id="504f7-109">For more information about authorization, see [Get access tokens to call Microsoft Graph](/graph/auth/).</span></span>

## <a name="common-dynamics-365-business-central-scenarios"></a><span data-ttu-id="504f7-110">Сценарии Common Dynamics 365 Business Central</span><span class="sxs-lookup"><span data-stu-id="504f7-110">Common Dynamics 365 Business Central scenarios</span></span>
<span data-ttu-id="504f7-111">Центр API Dynamics 365 позволяет читать и изменять бизнес-данные с помощью приложений, подключенных и интегрированных через одну конечную точку.</span><span class="sxs-lookup"><span data-stu-id="504f7-111">The Dynamics 365 Business Central API allows you to read and modify business data through apps that are connected and integrated through a single endpoint.</span></span> <span data-ttu-id="504f7-112">Используйте API, чтобы, например, [](../resources/dynamics-customer.md) получить [](../resources/dynamics-vendor.md) доступ к сведениям о клиентах и поставщиках или [просмотреть просроченные платежи.](../resources/dynamics-agedaccountspayable.md)</span><span class="sxs-lookup"><span data-stu-id="504f7-112">Use the API to, for example, get access to [customer](../resources/dynamics-customer.md) and [vendor](../resources/dynamics-vendor.md) information, or [view overdue payments](../resources/dynamics-agedaccountspayable.md).</span></span>

## <a name="whats-new"></a><span data-ttu-id="504f7-113">Новые возможности</span><span class="sxs-lookup"><span data-stu-id="504f7-113">What's new</span></span>
<span data-ttu-id="504f7-114">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="504f7-114">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="504f7-115">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="504f7-115">Next steps</span></span>
<span data-ttu-id="504f7-116">Центр API Dynamics 365 может открыть новые способы для работы с пользователями.</span><span class="sxs-lookup"><span data-stu-id="504f7-116">The Dynamics 365 Business Central API can open up new ways for you to engage with users.</span></span> <span data-ttu-id="504f7-117">Дополнительные сведения см. в следующих источниках.</span><span class="sxs-lookup"><span data-stu-id="504f7-117">To learn more, see the following:</span></span>

+ [<span data-ttu-id="504f7-118">Обзор центра бизнеса Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="504f7-118">Dynamics 365 Business Central Overview</span></span>](/graph/dynamics-business-central-concept-overview)
+ <span data-ttu-id="504f7-119">Попробуйте [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="504f7-119">Try [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<!--
|For Resource Type |See                                                 |
|:-----------------|:---------------------------------------------------|
|account resource type|[account](../resources/dynamics-account.md)|
|aged accounts receivable resource type|[agedAccountsReceivable](../resources/dynamics-agedaccountsreceivable.md)|
|aged accounts payable resource type|[agedAccountsPayable](../resources/dynamics-agedaccountspayable.md)|
|balance sheet resource type|[balanceSheet](../resources/dynamics-balancesheet.md)|
|companies resource type|[companies](../resources/dynamics-companies.md)|
|companyInformation resource type|[companyInformation](../resources/dynamics-companyinformation.md)|
|countriesRegions resource type|[countriesRegions](../resources/dynamics-countriesregions.md)|
|currencies resource type|[currencies](../resources/dynamics-currencies.md)|
|customer resource type|[customer](../resources/dynamics-customer.md)|
|customerPaymentJournal resource type|[customerPaymentsJournal](../resources/dynamics-customerpaymentsjournal.md)|
|customerPayment resource type|[customerPayment](../resources/dynamics-customerpayment.md)|
|dimension resource type|[dimension](../resources/dynamics-dimension.md)|
|dimensionValue resource type|[dimensionValue](../resources/dynamics-dimensionvalue.md)
|employee resource type|[employee](../resources/dynamics-employee.md)|
|generalLedgerEntries resource type|[generalLedgerEntries](../resources/dynamics-generalledgerentries.md)|
|item resource type|[item](../resources/dynamics-item.md)|
|itemCategories resource type|[itemCategories](../resources/dynamics-itemcategories.md)|
|income statement resource type|[incomeStatement](../resources/dynamics-incomestatement.md)|
|IRS1099 resource type|[irs1099](../resources/dynamics-irs1099.md)|
|journal resource type|[journal](../resources/dynamics-journal.md)|
|journalLine resource type|[journalLine](../resources/dynamics-journalline.md)|
|paymentMethods resource type|[paymentMethods](../resources/dynamics-paymentmethods.md)|
|paymentTerms resource type|[paymentTerms](../resources/dynamics-paymentterms.md)|
|retained earnings statement resource type|[retainedEarningsStatement](../resources/dynamics-retainedearningsstatement.md)|
|shipmentMethods resource type|[shipmentMethods](../resources/dynamics-shipmentmethods.md)|
|taxGroups resource type|[taxGroups](../resources/dynamics-taxgroups.md)|
|taxArea resource type|[taxAreas](..resources/dynamics-taxarea.md)|
|unitsOfMeasure resource type|[unitsOfMeasure](../resources/dynamics-unitsofmeasure.md)|
|vendor resource type|[vendor](../resources/dynamics-vendor.md)|
-->