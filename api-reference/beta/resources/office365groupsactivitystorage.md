---
title: Тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: a3168ad417f246017ba1018aca265ec0363c951e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009463"
---
# <a name="office365groupsactivitystorage-resource-type"></a>Тип ресурса office365GroupsActivityStorage

## <a name="properties"></a>Свойства

| Свойство                  | Тип   | Описание                              |
| :------------------------ | :----- | ---------------------------------------- |
| Репортрефрешдате         | Дата   | Самая поздняя дата контента.          |
| Маилбокссторажеусединбитес | Int64  | Хранилище, используемое в почтовом ящике группы.       |
| Ситесторажеусединбитес    | Int64  | Хранилище, используемое в библиотеке документов SharePoint. |
| reportDate                | Дата   | Дата моментального снимка хранилища для Exchange и SharePoint. |
| Репортпериод              | String | Количество дней, охватываемых отчетом.    |

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
