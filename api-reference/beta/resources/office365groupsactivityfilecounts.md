---
title: тип ресурса office365GroupsActivityFileCounts
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 0c7d2b89dde8e288fb8ca81dc7ca67e6830a4122
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59142833"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>тип ресурса office365GroupsActivityFileCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Дата   | Последняя дата контента.          |
| total             | Int64  | Общее число файлов в библиотеке SharePoint группы. |
| active            | Int64  | Количество файлов, которые просматривались, редактировали, делились или синхронизировались в библиотеке документов SharePoint группы. |
| reportDate        | Дата   | Дата активных действий нескольких файлов на веб-сайте SharePoint группы. |
| reportPeriod      | String | Количество дней, которые охватывает отчет.    |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {

  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


