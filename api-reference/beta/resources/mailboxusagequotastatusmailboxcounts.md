---
title: Тип ресурса mailboxUsageQuotaStatusMailboxCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: b87bb1ce91626f9151d294e2243bba72ba72346b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835225"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a>Тип ресурса mailboxUsageQuotaStatusMailboxCounts

## <a name="properties"></a>Свойства

| Свойство              | Тип   |
| :-------------------- | :----- |
| reportRefreshDate     | Date   |
| underLimit            | Int64  |
| warningIssued         | Int64  |
| sendProhibited        | Int64  |
| sendReceiveProhibited | Int64  |
| неопределенное         | Int64  |
| reportDate            | Date   |
| reportPeriod          | String |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageQuotaStatusMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "underLimit": 1024, 
  "warningIssued": 1024, 
  "sendProhibited": 1024, 
  "sendReceiveProhibited": 1024, 
  "indeterminate": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
