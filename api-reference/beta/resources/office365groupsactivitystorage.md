---
title: Тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0485fd95046bc83350983bc1333dba83c79139d6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505552"
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
