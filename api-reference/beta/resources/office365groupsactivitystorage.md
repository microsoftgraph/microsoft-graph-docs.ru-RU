---
title: Тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: 9824d3d172a8578f8a25a049c2d0d3b407bbc47e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862253"
---
# <a name="office365groupsactivitystorage-resource-type"></a>Тип ресурса office365GroupsActivityStorage

## <a name="properties"></a>Свойства

| Свойство                  | Тип   | Описание                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | Date   | Последняя дата контента.          |
| mailboxStorageUsedInBytes | Int64  | Используются в почтовом ящике группы хранения.       |
| siteStorageUsedInBytes    | Int64  | Хранения, используемый в библиотеке документов SharePoint. |
| reportDate                | Date   | Дата моментальный снимок для Exchange и SharePoint используется хранилища. |
| reportPeriod              | Строка | Количество дней, на которое отчета.    |

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
