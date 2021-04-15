---
title: тип ресурса teamsUserActivityUserCounts
description: Представляет число ежедневных пользователей по типу действия.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f1ddb3e6e5e6a0b6fbb5c9973bec7e29f4492089
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766443"
---
# <a name="teamsuseractivityusercounts-resource-type"></a>тип ресурса teamsUserActivityUserCounts

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет число ежедневных пользователей по типу действия.

## <a name="properties"></a>Свойства

| Свойство            | Тип   | Описание                                                  |
| :------------------ | :----- | ------------------------------------------------------------ |
| reportRefreshDate   | Дата   | Последняя дата контента.                              |
| reportDate          | Дата   | Дата выполнения пользователями действий.        |
| teamChatMessages    | Int64  | Количество пользователей, которые разместили сообщение в командном чате.       |
| privateChatMessages | Int64  | Число пользователей, которые разместили сообщение в частном чате.    |
| calls               | Int64  | Число пользователей, которые участвовали в звонках 1:1.           |
| meetings            | Int64  | Количество пользователей, которые участвовали в собраниях в Интернете.     |
| otherActions        | Int64  | Число пользователей, которые были активными, но выполняли другие действия, чем выставленные типы действий, предлагаемые в отчете (отправка или ответ на сообщения канала и сообщения чата, планирование или участие в звонках и собраниях 1:1). Примеры действий, когда пользователь меняет состояние Teams или сообщение о состоянии Teams или открывает сообщение сообщения канала, но не отвечает. |
| reportPeriod        | String | Количество дней, которые охватывает отчет.                        |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```


