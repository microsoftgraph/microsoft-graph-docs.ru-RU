---
title: Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1ebbfe0f134848d78e9c42a159c1c56bdbd21b39
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473427"
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
