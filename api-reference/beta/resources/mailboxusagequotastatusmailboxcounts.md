---
title: Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ce215e0eae3a13aa0c2d27f54338efc57c0c5486
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522843"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a>Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс

Пространство имен: Microsoft. Graph

## <a name="properties"></a>Свойства

| Свойство              | Тип   |
| :-------------------- | :----- |
| репортрефрешдате     | Дата   |
| поддельное значение            | Int64  |
| варнингиссуед         | Int64  |
| сендпрохибитед        | Int64  |
| сендрецеивепрохибитед | Int64  |
| определен         | Int64  |
| reportDate            | Дата   |
| репортпериод          | String |

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
