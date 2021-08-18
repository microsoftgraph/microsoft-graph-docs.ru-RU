---
title: тип ресурса office365GroupsActivityFileCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: f05cf16e1b2e0273aaa62241bbeac3b0d872bf87605e2c852ac2ab28e25f9526
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54160865"
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
| reportPeriod      | Строка | Количество дней, которые охватывает отчет.    |

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


