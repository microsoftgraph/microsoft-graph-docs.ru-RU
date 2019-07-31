---
title: Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1e8fafe9a3cdce4519cf5755337b016fa587cd06
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966904"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a>Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс

## <a name="properties"></a>Свойства

| Свойство              | Тип   |
| :-------------------- | :----- |
| Репортрефрешдате     | Дата   |
| поддельное значение            | Int64  |
| Варнингиссуед         | Int64  |
| Сендпрохибитед        | Int64  |
| Сендрецеивепрохибитед | Int64  |
| определен         | Int64  |
| reportDate            | Дата   |
| Репортпериод          | String |

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
