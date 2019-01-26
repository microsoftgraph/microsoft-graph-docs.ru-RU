---
title: Тип ресурса office365GroupsActivityGroupCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: b202d5189c1edeeeaa45d447aa7cc078dd263858
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572488"
---
# <a name="office365groupsactivitygroupcounts-resource-type"></a>Тип ресурса office365GroupsActivityGroupCounts

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Date   | Последняя дата контента.          |
| total             | Int64  | Общее число групп.              |
| активных            | Int64  | Число активных групп. Группы считается активным, если какие-либо из следующих значений: групповой полученных почтового ящика электронной почты; пользователю просматривать, редактировать, общих или синхронизирован файлы в библиотеке документов SharePoint. пользователь просматривает страницы SharePoint; пользователь учтена, чтение или оцененных сообщений в группах Yammer. |
| reportDate        | Date   | Дата, на котором выполнялись число групп. |
| reportPeriod      | Строка | Количество дней, на которое отчета.    |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts"
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
