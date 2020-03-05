---
title: Тип ресурса Яммерграупсактивитидетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 9363bd711900cc6211e995c112581d3a91e08a04
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518989"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>Тип ресурса Яммерграупсактивитидетаил

Пространство имен: Microsoft. Graph

## <a name="properties"></a>Свойства

| Свойство           | Тип    |
| :----------------- | :------ |
| репортрефрешдате  | Дата    |
| граупдисплайнаме   | String  |
| isDeleted          | Логический |
| овнерпринЦипалнаме | String  |
| ластактивитидате   | Дата    |
| groupType          | String  |
| office365Connected | Логический |
| мемберкаунт        | Int64   |
| постедкаунт        | Int64   |
| реадкаунт          | Int64   |
| ликедкаунт         | Int64   |
| репортпериод       | String  |

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
