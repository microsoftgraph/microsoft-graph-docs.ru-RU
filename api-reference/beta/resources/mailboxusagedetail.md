---
title: Тип ресурса Маилбоксусажедетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e630a64e7ece98d956a5f3821ec92413512fc7e4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966939"
---
# <a name="mailboxusagedetail-resource-type"></a>Тип ресурса Маилбоксусажедетаил

## <a name="properties"></a>Свойства

| Свойство                        | Тип    |
| :------------------------------ | :------ |
| Репортрефрешдате               | Дата    |
| userPrincipalName               | String  |
| displayName                     | Строка  |
| isDeleted                       | Boolean |
| Делетеддате                     | Дата    |
| createdDate                     | Дата    |
| Ластактивитидате                | Дата    |
| itemCount                       | Int64   |
| Сторажеусединбитес              | Int64   |
| Делетедитемкаунт                | Int64   |
| Делетедитемсизеинбитес          | Int64   |
| Иссуеварнингкуотаинбитес        | Int64   |
| Прохибитсендкуотаинбитес        | Int64   |
| Прохибитсендрецеивекуотаинбитес | Int64   |
| Репортпериод                    | String  |

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
