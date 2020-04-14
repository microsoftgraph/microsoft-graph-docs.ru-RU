---
title: Тип ресурса Маилбоксусажедетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 485dba38275cb437f069abf1309bdc0705ad967a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473481"
---
# <a name="mailboxusagedetail-resource-type"></a>Тип ресурса Маилбоксусажедетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                        | Тип    |
| :------------------------------ | :------ |
| репортрефрешдате               | Дата    |
| userPrincipalName               | String  |
| displayName                     | Строка  |
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

## <a name="json-representation"></a>Представление JSON

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
