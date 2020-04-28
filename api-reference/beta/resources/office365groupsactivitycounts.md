---
title: Тип ресурса office365GroupsActivityCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: f07743a592753daff2670478c6f2fe18207f6013
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522458"
---
# <a name="office365groupsactivitycounts-resource-type"></a>Тип ресурса office365GroupsActivityCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство               | Тип   | Описание                              |
| :--------------------- | :----- | ---------------------------------------- |
| репортрефрешдате      | Дата   | Самая поздняя дата контента.          |
| ексчанжеемаилсрецеивед | Int64  | Количество сообщений электронной почты, получаемых групповой почтовыми ящиками. |
| яммермессажеспостед   | Int64  | Количество сообщений, отправленных в группы Yammer. |
| яммермессажесреад     | Int64  | Количество сообщений, прочитанных в группах Yammer. |
| яммермессажесликед    | Int64  | Количество сообщений, которые понравилось в группах Yammer. |
| reportDate             | Дата   | Дата, когда в группу Yammer было отправлено, прочитано или понравилось количество сообщений электронной почты для почтового ящика группы или сообщений. |
| репортпериод           | String | Количество дней, охватываемых отчетом.    |

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
