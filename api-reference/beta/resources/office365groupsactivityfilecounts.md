---
title: Тип ресурса office365GroupsActivityFileCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 856bb4c74c8af35775b6fe71cb75d89935440bdb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819188"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>Тип ресурса office365GroupsActivityFileCounts

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Date   | Последняя дата контента.          |
| total             | Int64  | Общее число файлов в библиотеке документов SharePoint группы. |
| активных            | Int64  | Число файлов, которые были просматривать, редактировать, общих или синхронизирован в библиотеке документов SharePoint группы. |
| reportDate        | Date   | Дата, на котором количество файлов были активны на сайте группы SharePoint. |
| reportPeriod      | Строка | Количество дней, на которое отчета.    |

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
