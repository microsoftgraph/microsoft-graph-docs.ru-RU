---
title: Работа с API Dynamics 365 Business Central в Microsoft Graph
description: Документация по API для интеграции с Microsoft Graph
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: conceptualPageType
ms.openlocfilehash: 5566c19288029e0607e2da60cde49e6bb9bb5471
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013855"
---
# <a name="working-with-the-dynamics-365-business-central-api-in-microsoft-graph"></a><span data-ttu-id="dd3a1-103">Работа с API Dynamics 365 Business Central в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="dd3a1-103">Working with the Dynamics 365 Business Central API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd3a1-104">Вы можете использовать Microsoft Graph для подключения и интеграции веб-службы или решения SaaS с Microsoft Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="dd3a1-104">You can use Microsoft Graph to connect and integrate your web service or SaaS solution with Microsoft Dynamics 365 Business Central.</span></span> <span data-ttu-id="dd3a1-105">С помощью Microsoft Graph вы можете создавать приложения, которые обеспечивают доступ к данным и тесно интегрируются с Microsoft Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="dd3a1-105">With Microsoft Graph, you can build apps that get authorized access to and integrate seamlessly with Microsoft Dynamics 365 Business Central data.</span></span>

## <a name="authorization"></a><span data-ttu-id="dd3a1-106">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd3a1-106">Authorization</span></span>
<span data-ttu-id="dd3a1-107">Используйте конечную точку Azure AD версии 2.0 для проверки подлинности в Dynamics 365 Business Central API.</span><span class="sxs-lookup"><span data-stu-id="dd3a1-107">Use the Azure AD v2.0 endpoint to authenticate Dynamics 365 Business Central APIs.</span></span> <span data-ttu-id="dd3a1-108">Для всех API требуется `Authorization: Bearer {access-token}` заголовок запроса.</span><span class="sxs-lookup"><span data-stu-id="dd3a1-108">All APIs require the `Authorization: Bearer {access-token}` request header.</span></span> <span data-ttu-id="dd3a1-109">Дополнительные сведения о проверке подлинности приведены [в разделе получение маркеров доступа для вызова Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="dd3a1-109">For more information about authorization, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span>

## <a name="common-dynamics-365-business-central-scenarios"></a><span data-ttu-id="dd3a1-110">Распространенные сценарии Dynamics 365 Business Central</span><span class="sxs-lookup"><span data-stu-id="dd3a1-110">Common Dynamics 365 Business Central scenarios</span></span>
<span data-ttu-id="dd3a1-111">API Dynamics 365 Business Central позволяет считывать и изменять бизнес-данные через приложения, которые подключены и интегрируются через одну конечную точку.</span><span class="sxs-lookup"><span data-stu-id="dd3a1-111">The Dynamics 365 Business Central API allows you to read and modify business data through apps that are connected and integrated through a single endpoint.</span></span> <span data-ttu-id="dd3a1-112">Используйте API, например, для получения доступа к сведениям о [клиентах](../resources/dynamics-customer.md) и [поставщиках](../resources/dynamics-vendor.md) или [просмотра просроченных платежей](../resources/dynamics-agedaccountspayable.md).</span><span class="sxs-lookup"><span data-stu-id="dd3a1-112">Use the API to, for example, get access to [customer](../resources/dynamics-customer.md) and [vendor](../resources/dynamics-vendor.md) information, or [view overdue payments](../resources/dynamics-agedaccountspayable.md).</span></span>

## <a name="whats-new"></a><span data-ttu-id="dd3a1-113">Новые возможности</span><span class="sxs-lookup"><span data-stu-id="dd3a1-113">What's new</span></span>
<span data-ttu-id="dd3a1-114">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="dd3a1-114">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="dd3a1-115">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="dd3a1-115">Next steps</span></span>
<span data-ttu-id="dd3a1-116">API Dynamics 365 Business Central может открыть новые способы взаимодействия с пользователями.</span><span class="sxs-lookup"><span data-stu-id="dd3a1-116">The Dynamics 365 Business Central API can open up new ways for you to engage with users.</span></span> <span data-ttu-id="dd3a1-117">Дополнительные сведения см. в следующих источниках.</span><span class="sxs-lookup"><span data-stu-id="dd3a1-117">To learn more, see the following:</span></span>

+ [<span data-ttu-id="dd3a1-118">Dynamics 365 Business Central Overview</span><span class="sxs-lookup"><span data-stu-id="dd3a1-118">Dynamics 365 Business Central Overview</span></span>](/graph/dynamics-business-central-concept-overview)
+ <span data-ttu-id="dd3a1-119">Попробуйте использовать [проводник Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="dd3a1-119">Try [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

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
|trial balance resource type|[trialBalance](../resources/dynamics-trialbalance.md)|
|unitsOfMeasure resource type|[unitsOfMeasure](../resources/dynamics-unitsofmeasure.md)|
|vendor resource type|[vendor](../resources/dynamics-vendor.md)|
-->


