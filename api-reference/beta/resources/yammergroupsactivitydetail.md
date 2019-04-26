---
title: Тип ресурса Яммерграупсактивитидетаил
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c5b580f643686c27497fd24a6fe00c7750a6a938
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551423"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>Тип ресурса Яммерграупсактивитидетаил

## <a name="properties"></a>Свойства

| Свойство           | Тип    |
| :----------------- | :------ |
| Репортрефрешдате  | Дата    |
| Граупдисплайнаме   | String  |
| isDeleted          | Логический |
| ОвнерпринЦипалнаме | String  |
| Ластактивитидате   | Дата    |
| groupType          | String  |
| office365Connected | Логический |
| Мемберкаунт        | Int64   |
| Постедкаунт        | Int64   |
| Реадкаунт          | Int64   |
| Ликедкаунт         | Int64   |
| Репортпериод       | String  |

## <a name="json-representation"></a>Представление в формате JSON

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
