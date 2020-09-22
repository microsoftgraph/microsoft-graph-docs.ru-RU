---
title: Тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 0b14e6981a193ad1698303d2762d0321de430b73
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092393"
---
# <a name="office365groupsactivitystorage-resource-type"></a>Тип ресурса office365GroupsActivityStorage

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                  | Тип   | Описание                              |
| :------------------------ | :----- | ---------------------------------------- |
| репортрефрешдате         | Дата   | Самая поздняя дата контента.          |
| маилбокссторажеусединбитес | Int64  | Хранилище, используемое в почтовом ящике группы.       |
| ситесторажеусединбитес    | Int64  | Хранилище, используемое в библиотеке документов SharePoint. |
| reportDate                | Дата   | Дата моментального снимка хранилища для Exchange и SharePoint. |
| репортпериод              | Строка | Количество дней, охватываемых отчетом.    |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailboxStorageUsedInBytes": 1024, 
  "siteStorageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


