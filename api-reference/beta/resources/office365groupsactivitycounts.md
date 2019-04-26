---
title: Тип ресурса office365GroupsActivityCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c94e79f688e117960b3a8a0f2c9888a908634a82
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581725"
---
# <a name="office365groupsactivitycounts-resource-type"></a>Тип ресурса office365GroupsActivityCounts

## <a name="properties"></a>Свойства

| Свойство               | Тип   | Описание                              |
| :--------------------- | :----- | ---------------------------------------- |
| Репортрефрешдате      | Дата   | Самая поздняя дата контента.          |
| Ексчанжеемаилсрецеивед | Int64  | Количество сообщений электронной почты, получаемых групповой почтовыми ящиками. |
| Яммермессажеспостед   | Int64  | Количество сообщений, отправленных в группы Yammer. |
| Яммермессажесреад     | Int64  | Количество сообщений, прочитанных в группах Yammer. |
| Яммермессажесликед    | Int64  | Количество сообщений, которые понравилось в группах Yammer. |
| reportDate             | Дата   | Дата, когда в группу Yammer было отправлено, прочитано или понравилось количество сообщений электронной почты для почтового ящика группы или сообщений. |
| Репортпериод           | String | Количество дней, охватываемых отчетом.    |

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
