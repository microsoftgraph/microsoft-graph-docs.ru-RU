---
title: тип ресурса teamsUserActivityDistributionUserCounts
description: Представляет число пользователей по типу действия за выбранный период времени.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3d4fa8b3aec98a03d7e51819db0dc4797367f499
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766985"
---
# <a name="teamsuseractivitydistributionusercounts-resource-type"></a>тип ресурса teamsUserActivityDistributionUserCounts

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет число пользователей по типу действия за выбранный период времени.

## <a name="properties"></a>Свойства

| Свойство            | Тип   | Описание                                                  |
| :------------------ | :----- | ------------------------------------------------------------ |
| reportRefreshDate   | Дата   | Последняя дата контента.                              |
| teamChatMessages    | Int64  | Количество уникальных сообщений, которые пользователи разместили в командном чате. |
| privateChatMessages | Int64  | Количество уникальных сообщений, которые пользователи разместили в частном чате. |
| calls               | Int64  | Количество уникальных вызовов 1:1, в которые участвовали пользователи.   |
| meetings            | Int64  | Количество уникальных онлайн-собраний, в которые участвовали пользователи. |
| reportPeriod        | String | Количество дней, которые охватывает отчет.                        |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityDistributionUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```


