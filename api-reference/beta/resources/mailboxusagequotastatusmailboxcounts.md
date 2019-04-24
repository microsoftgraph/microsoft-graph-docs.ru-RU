---
title: Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 45e4754fef0dd3a2f7a669e3b3b96692d117c8f0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457132"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a>Тип ресурса Маилбоксусажекуотастатусмаилбокскаунтс

## <a name="properties"></a>Свойства

| Свойство              | Тип   |
| :-------------------- | :----- |
| Репортрефрешдате     | Дата   |
| подДельное значение            | Int64  |
| Варнингиссуед         | Int64  |
| Сендпрохибитед        | Int64  |
| Сендрецеивепрохибитед | Int64  |
| определен         | Int64  |
| reportDate            | Дата   |
| Репортпериод          | Строка |

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
