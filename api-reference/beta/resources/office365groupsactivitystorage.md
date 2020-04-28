---
title: Тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: ba81621a819bb38f2d5d48e118729fc4476b5806
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522430"
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
| репортпериод              | String | Количество дней, охватываемых отчетом.    |

## <a name="json-representation"></a>Представление JSON

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
