---
title: Тип ресурса Маилбоксусажедетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: bea72f49f1cefc7874d9a5aa7e92e7dcd7caaa71
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055234"
---
# <a name="mailboxusagedetail-resource-type"></a>Тип ресурса Маилбоксусажедетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                        | Тип    |
| :------------------------------ | :------ |
| репортрефрешдате               | Дата    |
| userPrincipalName               | String  |
| displayName                     | String  |
| isDeleted                       | Boolean |
| делетеддате                     | Дата    |
| createdDate                     | Дата    |
| ластактивитидате                | Дата    |
| itemCount                       | Int64   |
| сторажеусединбитес              | Int64   |
| делетедитемкаунт                | Int64   |
| делетедитемсизеинбитес          | Int64   |
| иссуеварнингкуотаинбитес        | Int64   |
| прохибитсендкуотаинбитес        | Int64   |
| прохибитсендрецеивекуотаинбитес | Int64   |
| репортпериод                    | String  |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "createdDate": "Date", 
  "lastActivityDate": "Date", 
  "itemCount": 1024, 
  "storageUsedInBytes": 1024, 
  "deletedItemCount": 1024,
  "deletedItemSizeInBytes": 1024, 
  "issueWarningQuotaInBytes": 1024, 
  "prohibitSendQuotaInBytes": 1024, 
  "prohibitSendReceiveQuotaInBytes": 1024, 
  "reportPeriod": "String"
}
```


