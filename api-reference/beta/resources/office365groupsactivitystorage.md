---
title: тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 1c0f62b2f8551e0e1931bf65d8ee592a3dc72373e1a6f41d37b167a3bdcef38b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54176332"
---
# <a name="office365groupsactivitystorage-resource-type"></a>тип ресурса office365GroupsActivityStorage

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                  | Тип   | Описание                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | Дата   | Последняя дата контента.          |
| mailboxStorageUsedInBytes | Int64  | Хранилище, используемого в групповом почтовом ящике.       |
| siteStorageUsedInBytes    | Int64  | Хранилище, используемого в SharePoint библиотеке документов. |
| reportDate                | Дата   | Дата снимка для Exchange и SharePoint используемого хранилища. |
| reportPeriod              | String | Количество дней, которые охватывает отчет.    |

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


