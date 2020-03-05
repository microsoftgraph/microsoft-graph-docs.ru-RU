---
title: Работа с API Dynamics 365 Business Central в Microsoft Graph
description: Документация по API для интеграции с Microsoft Graph
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: conceptualPageType
ms.openlocfilehash: 97031294aa27ef18e2043f8250c6c6c893e3539d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503910"
---
# <a name="working-with-the-dynamics-365-business-central-api-in-microsoft-graph"></a>Работа с API Dynamics 365 Business Central в Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете использовать Microsoft Graph для подключения и интеграции веб-службы или решения SaaS с Microsoft Dynamics 365 Business Central. С помощью Microsoft Graph вы можете создавать приложения, которые обеспечивают доступ к данным и тесно интегрируются с Microsoft Dynamics 365 Business Central.

## <a name="authorization"></a>Authorization
Используйте конечную точку Azure AD версии 2.0 для проверки подлинности в Dynamics 365 Business Central API. Для `Authorization: Bearer {access-token}` всех API требуется заголовок запроса. Дополнительные сведения о проверке подлинности приведены [в разделе получение маркеров доступа для вызова Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).

## <a name="common-dynamics-365-business-central-scenarios"></a>Распространенные сценарии Dynamics 365 Business Central
API Dynamics 365 Business Central позволяет считывать и изменять бизнес-данные через приложения, которые подключены и интегрируются через одну конечную точку. Используйте API, например, для получения доступа к сведениям о [клиентах](../resources/dynamics-customer.md) и [поставщиках](../resources/dynamics-vendor.md) или [просмотра просроченных платежей](../resources/dynamics-agedaccountspayable.md).

## <a name="next-steps"></a>Дальнейшие действия
API Dynamics 365 Business Central может открыть новые способы взаимодействия с пользователями. Дополнительные сведения см. в следующих источниках.

+ [Dynamics 365 Business Central Overview](/graph/dynamics-business-central-concept-overview)
+ Попробуйте использовать [проводник Graph](https://developer.microsoft.com/graph/graph-explorer).

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
