---
title: Тип ресурса office365GroupsActivityStorage
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 23ff4d112373f52c4c19d6631ac89bac22399b29
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081592"
---
# <a name="office365groupsactivitystorage-resource-type"></a>Тип ресурса office365GroupsActivityStorage

## <a name="properties"></a>Свойства

| Свойство                  | Тип   | Description                              |
| :------------------------ | :----- | ---------------------------------------- |
| reportRefreshDate         | Date   | Последняя дата контента.          |
| mailboxStorageUsedInBytes | Int64  | Используются в почтовом ящике группы хранения.       |
| siteStorageUsedInBytes    | Int64  | Хранения, используемый в библиотеке документов SharePoint. |
| reportDate                | Date   | Дата моментальный снимок для Exchange и SharePoint используется хранилища. |
| reportPeriod              | String | Количество дней, на которое отчета.    |

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
