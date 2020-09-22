---
title: Тип ресурса office365GroupsActivityFileCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: c887ecb526d9c4215c1d8586bcbcb799c9e2c476
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092407"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>Тип ресурса office365GroupsActivityFileCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| репортрефрешдате | Дата   | Самая поздняя дата контента.          |
| total             | Int64  | Общее количество файлов в библиотеке документов SharePoint группы. |
| ASP            | Int64  | Количество файлов, которые были просмотрены, изменены, предоставлены в общий доступ или синхронизированы в библиотеке документов SharePoint группы. |
| reportDate        | Дата   | Дата, когда число файлов было активно на сайте SharePoint группы. |
| репортпериод      | Строка | Количество дней, охватываемых отчетом.    |

## <a name="json-representation"></a>Представление в формате JSON

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


