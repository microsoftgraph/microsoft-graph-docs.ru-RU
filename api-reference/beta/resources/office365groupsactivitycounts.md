---
title: Тип ресурса office365GroupsActivityCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c94e79f688e117960b3a8a0f2c9888a908634a82
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572334"
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
