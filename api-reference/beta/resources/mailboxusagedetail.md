---
title: Тип ресурса Маилбоксусажедетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 2890205db7cec6f20eef17c24da112517bf169a1
ms.sourcegitcommit: 6fe086e6a9396a71a82179853547cb7b5e22d980
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/20/2019
ms.locfileid: "35805223"
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
