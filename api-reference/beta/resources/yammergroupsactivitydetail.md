---
title: Тип ресурса Яммерграупсактивитидетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 2188cf1ad583ba66fffb1d7b86009f49fba3f8fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046077"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>Тип ресурса Яммерграупсактивитидетаил

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство           | Тип    |
| :----------------- | :------ |
| репортрефрешдате  | Дата    |
| граупдисплайнаме   | Строка  |
| isDeleted          | Boolean |
| овнерпринЦипалнаме | Строка  |
| ластактивитидате   | Дата    |
| groupType          | Строка  |
| office365Connected | Boolean |
| мемберкаунт        | Int64   |
| постедкаунт        | Int64   |
| реадкаунт          | Int64   |
| ликедкаунт         | Int64   |
| нетворкдисплайнаме | Строка  |
| репортпериод       | Строка  |

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


