---
title: Тип ресурса yammerGroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c5b580f643686c27497fd24a6fe00c7750a6a938
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573265"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>Тип ресурса yammerGroupsActivityDetail

## <a name="properties"></a>Свойства

| Свойство           | Тип    |
| :----------------- | :------ |
| reportRefreshDate  | Date    |
| groupDisplayName   | Строка  |
| isDeleted          | Boolean |
| ownerPrincipalName | Строка  |
| lastActivityDate   | Date    |
| groupType          | Строка  |
| office365Connected | Boolean |
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
