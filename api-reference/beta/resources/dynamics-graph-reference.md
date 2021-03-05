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
# <a name="working-with-the-dynamics-365-business-central-api-in-microsoft-graph"></a>Работа с центральным API Dynamics 365 в Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете использовать Microsoft Graph для подключения и интеграции веб-службы или решения SaaS с Microsoft Dynamics 365 Business Central. С помощью Microsoft Graph можно создавать приложения, которые получают авторизованный доступ к данным Microsoft Dynamics 365 Business Central и интегрируются с ними без проблем.

## <a name="authorization"></a>Авторизация
Используйте конечную точку Azure AD v2.0 для проверки подлинности API Dynamics 365 Business Central. Все API требуют `Authorization: Bearer {access-token}` загона запроса. Дополнительные сведения о авторизации см. в записи [Get access tokens to call Microsoft Graph.](/graph/auth/)

## <a name="common-dynamics-365-business-central-scenarios"></a>Сценарии Common Dynamics 365 Business Central
Центр API Dynamics 365 позволяет читать и изменять бизнес-данные с помощью приложений, подключенных и интегрированных через одну конечную точку. Используйте API, чтобы, например, [](../resources/dynamics-customer.md) получить [](../resources/dynamics-vendor.md) доступ к сведениям о клиентах и поставщиках или [просмотреть просроченные платежи.](../resources/dynamics-agedaccountspayable.md)

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

## <a name="next-steps"></a>Дальнейшие действия
Центр API Dynamics 365 может открыть новые способы для работы с пользователями. Дополнительные сведения см. в следующих источниках.

+ [Обзор центра бизнеса Dynamics 365](/graph/dynamics-business-central-concept-overview)
+ Попробуйте [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).

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