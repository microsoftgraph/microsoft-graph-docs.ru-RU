---
title: Тип ресурса Яммерграупсактивитидетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: f16eda3f28556a18c47c68d532ace4244edfad19
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963754"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>Тип ресурса Яммерграупсактивитидетаил

## <a name="properties"></a>Свойства

| Свойство           | Тип    |
| :----------------- | :------ |
| Репортрефрешдате  | Дата    |
| Граупдисплайнаме   | String  |
| isDeleted          | Boolean |
| ОвнерпринЦипалнаме | String  |
| Ластактивитидате   | Дата    |
| groupType          | String  |
| office365Connected | Boolean |
| Мемберкаунт        | Int64   |
| Постедкаунт        | Int64   |
| Реадкаунт          | Int64   |
| Ликедкаунт         | Int64   |
| Репортпериод       | String  |

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
