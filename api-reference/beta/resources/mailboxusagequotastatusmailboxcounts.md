---
title: Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e09b9d27da4a85dd89f6a09440d56532045573b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029178"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a>Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс

Пространство имен: microsoft.graph

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


