---
title: тип ресурса yammerGroupsActivityDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 7c3b10b7b96c40ae7b7404eee2c9af99ea4bc2d602c93f9f6c68ef2ed7ad8cbe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54176087"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>тип ресурса yammerGroupsActivityDetail

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство           | Тип    |
| :----------------- | :------ |
| reportRefreshDate  | Дата    |
| groupDisplayName   | Строка  |
| isDeleted          | Логический |
| ownerPrincipalName | Строка  |
| lastActivityDate   | Дата    |
| groupType          | String  |
| office365Connected | Логический |
| memberCount        | Int64   |
| postedCount        | Int64   |
| readCount          | Int64   |
| likedCount         | Int64   |
| networkDisplayName | String  |
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
  "networkDisplayName": "String",
  "reportPeriod": "String"
}
```


