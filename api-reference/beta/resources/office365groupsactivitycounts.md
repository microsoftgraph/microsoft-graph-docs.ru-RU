---
title: тип ресурса office365GroupsActivityCounts
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: eed42f5baf9a0130c69f9f8e6c026c9e0082d200
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115123"
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
| reportPeriod           | String | Количество дней, которые охватывает отчет.    |

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


