---
title: тип ресурса office365GroupsActivityGroupCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: b7f38f2279e7cd575972d13ea411d972349131a4fe3a9943c4e5efa03365ffa2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178712"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a>тип ресурса office365GroupsActivityGroupCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Дата   | Последняя дата контента.          |
| total             | Int64  | Общее число групп.              |
| active            | Int64  | Количество активных групп. Группа считается активной, если произошло следующее: почтовый ящик группы получил электронную почту; просмотр, редактирование, общий доступ или синхронизацию файлов в SharePoint документа; просмотр страниц SharePoint пользователя; сообщений, которые пользователи вывешив, прочитав или понравились в Yammer группах. |
| reportDate        | Дата   | Дата активных действий ряда групп. |
| reportPeriod      | Строка | Количество дней, которые охватывает отчет.    |

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


