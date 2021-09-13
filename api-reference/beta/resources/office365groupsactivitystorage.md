---
title: тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 8a4e2159bcdb88401849352cd17012339c2ac8d4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115116"
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


