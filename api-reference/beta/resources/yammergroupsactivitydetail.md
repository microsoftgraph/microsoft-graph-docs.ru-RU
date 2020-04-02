---
title: Тип ресурса Яммерграупсактивитидетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 66e1817fa327444b51028292bcda59c8663bd683
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108419"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>Тип ресурса Яммерграупсактивитидетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство           | Тип    |
| :----------------- | :------ |
| репортрефрешдате  | Дата    |
| граупдисплайнаме   | String  |
| isDeleted          | Boolean |
| овнерпринЦипалнаме | String  |
| ластактивитидате   | Дата    |
| groupType          | String  |
| office365Connected | Boolean |
| мемберкаунт        | Int64   |
| постедкаунт        | Int64   |
| реадкаунт          | Int64   |
| ликедкаунт         | Int64   |
| нетворкдисплайнаме | String  |
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
  "networkDisplayName": "String",
  "reportPeriod": "String"
}
```
