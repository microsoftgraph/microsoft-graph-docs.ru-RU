---
title: Тип ресурса office365GroupsActivityFileCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 1f4f26e141dc25e1e5e249ad116bc9a988274f18
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981503"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a>Тип ресурса office365GroupsActivityFileCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Дата   | Последняя дата содержимого.          |
| total             | Int64  | Общее количество файлов в библиотеке документов SharePoint группы. |
| active            | Int64  | Количество файлов, которые просматривались, редактируются, совместно или синхронизированы в библиотеке документов SharePoint группы. |
| reportDate        | Дата   | Дата, когда на сайте SharePoint группы было активно несколько файлов. |
| reportPeriod      | String | Количество дней в отчете.    |

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


