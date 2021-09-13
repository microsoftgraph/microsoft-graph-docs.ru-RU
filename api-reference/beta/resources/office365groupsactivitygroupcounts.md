---
title: тип ресурса office365GroupsActivityGroupCounts
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 6548d32250d99a99f83e98d40c40041102caeb16
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59105785"
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
| reportPeriod      | String | Количество дней, которые охватывает отчет.    |

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


