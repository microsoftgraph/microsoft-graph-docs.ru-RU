---
title: Тип ресурса office365GroupsActivityCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 87867071545a36f7aca1833a369f919317153bc6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874111"
---
# <a name="office365groupsactivitycounts-resource-type"></a>Тип ресурса office365GroupsActivityCounts

## <a name="properties"></a>Свойства

| Свойство               | Тип   | Описание                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | Date   | Последняя дата контента.          |
| exchangeEmailsReceived | Int64  | Количество почтовых ящиков групп, получаемые по электронной почте. |
| yammerMessagesPosted   | Int64  | Число сообщений, помещенных в группы Yammer. |
| yammerMessagesRead     | Int64  | Количество сообщений, ознакомьтесь с разделом в группы Yammer. |
| yammerMessagesLiked    | Int64  | Количество сообщений, оцененных в группах Yammer. |
| reportDate             | Date   | Дата отправки целого ряда по электронной почте в почтовый ящик группы или учета количество сообщений, чтение или нравится, что в группе Yammer |
| reportPeriod           | Строка | Количество дней, на которое отчета.    |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeEmailsReceived": 1024, 
  "yammerMessagesPosted": 1024, 
  "yammerMessagesRead": 1024, 
  "yammerMessagesLiked": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
