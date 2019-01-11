---
title: Тип ресурса yammerGroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 9e4ac61f2af69b4229c2e9c3df7c653428cc2033
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832034"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>Тип ресурса yammerGroupsActivityDetail

## <a name="properties"></a>Свойства

| Свойство           | Тип    |
| :----------------- | :------ |
| reportRefreshDate  | Date    |
| groupDisplayName   | Строка  |
| isDeleted          | Логический |
| ownerPrincipalName | Строка  |
| lastActivityDate   | Date    |
| groupType          | Строка  |
| office365Connected | Логический |
| memberCount        | Int64   |
| postedCount        | Int64   |
| readCount          | Int64   |
| likedCount         | Int64   |
| reportPeriod       | String  |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "office365Connected": true, 
  "memberCount": 1024, 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "reportPeriod": "String"
}
```
