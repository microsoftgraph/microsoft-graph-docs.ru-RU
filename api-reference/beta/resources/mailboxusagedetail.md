---
title: Тип ресурса Маилбоксусажедетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 63b4b997a0ae559338fffd2acfabaa35dcc306e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581270"
---
# <a name="mailboxusagedetail-resource-type"></a>Тип ресурса Маилбоксусажедетаил

## <a name="properties"></a>Свойства

| Свойство                        | Тип    |
| :------------------------------ | :------ |
| Репортрефрешдате               | Дата    |
| userPrincipalName               | String  |
| displayName                     | String  |
| isDeleted                       | Boolean |
| Делетеддате                     | Дата    |
| createdDate                     | Дата    |
| Ластактивитидате                | Дата    |
| itemCount                       | Int64   |
| Сторажеусединбитес              | Int64   |
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
  "issueWarningQuotaInBytes": 1024, 
  "prohibitSendQuotaInBytes": 1024, 
  "prohibitSendReceiveQuotaInBytes": 1024, 
  "reportPeriod": "String"
}
```
