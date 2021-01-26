---
title: Тип ресурса office365GroupsActivityGroupCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: ad2610f5cbd3aae56651a0a5651e4ee4319b3bb2
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981496"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a>Тип ресурса office365GroupsActivityGroupCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Дата   | Последняя дата содержимого.          |
| total             | Int64  | Общее количество групп.              |
| active            | Int64  | Количество активных групп. Группа считается активной при любом из следующих действий: почтовый ящик группы, полученный по электронной почте; просматриваются, редактируются, совместно или синхронизируются файлы в библиотеке документов SharePoint; просматривались пользователем страницы SharePoint; пользователи опубликовали, прочитали или понравились сообщения в группах Yammer. |
| reportDate        | Дата   | Дата, когда было активно несколько групп. |
| reportPeriod      | String | Количество дней в отчете.    |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
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


