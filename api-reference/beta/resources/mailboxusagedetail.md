---
title: Тип ресурса Маилбоксусажедетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9c84ee4f36dac10499d553333654635934ca01a6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522864"
---
# <a name="mailboxusagedetail-resource-type"></a>Тип ресурса Маилбоксусажедетаил

Пространство имен: Microsoft. Graph

## <a name="properties"></a>Свойства

| Свойство                        | Тип    |
| :------------------------------ | :------ |
| репортрефрешдате               | Дата    |
| userPrincipalName               | String  |
| displayName                     | Строка  |
| isDeleted                       | Логический |
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
