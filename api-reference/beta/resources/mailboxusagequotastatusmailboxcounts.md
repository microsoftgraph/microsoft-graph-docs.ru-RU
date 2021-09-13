---
title: тип ресурса mailboxUsageQuotaStatusMailboxCounts
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4c26ddac97ecb3de1b35932a4b5c70869c502497
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033387"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a>тип ресурса mailboxUsageQuotaStatusMailboxCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство              | Тип   |
| :-------------------- | :----- |
| reportRefreshDate     | Дата   |
| underLimit            | Int64  |
| warningIssued         | Int64  |
| sendProhibited        | Int64  |
| sendReceiveProhibited | Int64  |
| indeterminate         | Int64  |
| reportDate            | Дата   |
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


