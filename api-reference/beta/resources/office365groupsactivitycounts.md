---
title: тип ресурса office365GroupsActivityCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 28ac5ad72a9e0b7e32336b397c0df114abf6fc9b88368f983dd84413ca4fe96e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226142"
---
# <a name="office365groupsactivitycounts-resource-type"></a>тип ресурса office365GroupsActivityCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство               | Тип   | Описание                              |
| :--------------------- | :----- | ---------------------------------------- |
| reportRefreshDate      | Дата   | Последняя дата контента.          |
| exchangeEmailsReceived | Int64  | Количество сообщений электронной почты, полученных почтовыми ящиками Группы. |
| yammerMessagesPosted   | Int64  | Количество сообщений, которые были размещены в Yammer группах. |
| yammerMessagesRead     | Int64  | Количество сообщений, читаемых в Yammer группах. |
| yammerMessagesLiked    | Int64  | Количество сообщений, которые нравятся в Yammer группах. |
| reportDate             | Дата   | Дата отправки нескольких электронных писем в групповой почтовый ящик или публикации нескольких сообщений в группе Yammer. |
| reportPeriod           | Строка | Количество дней, которые охватывает отчет.    |

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


