---
title: Тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 7ac9ca260e4723f7c4aeca8e15f837d4cd57b7c4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982182"
---
# <a name="office365groupsactivitystorage-resource-type"></a>Тип ресурса office365GroupsActivityStorage

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                  | Тип   | Описание                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | Дата   | Последняя дата содержимого.          |
| mailboxStorageUsedInBytes | Int64  | Хранилище, используемого в почтовом ящике группы.       |
| siteStorageUsedInBytes    | Int64  | Хранилище, используемого в библиотеке документов SharePoint. |
| reportDate                | Дата   | Моментальный снимок используемого хранилища Exchange и SharePoint. |
| reportPeriod              | String | Количество дней в отчете.    |

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


