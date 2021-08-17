---
title: тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: de01adee754940bd43be258b4454b7c68c0e4f8254581486d59a34f9a1f06478
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54139146"
---
# <a name="office365activationsusercounts-resource-type"></a>тип ресурса office365ActivationsUserCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                 | Тип   | Описание                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Дата   | Последняя дата контента.          |
| productType              | Строка | Тип продукта, например "Microsoft 365 ProPlus" или "Project клиент". |
| назначено                 | Int64  | Количество пользователей назначено для лицензии на продукт. |
| активирована                | Int64  | Количество пользователей, активировавших продукт. |
| sharedComputerActivation | Int64  | Число пользователей, которые использовали продукт на совместном компьютере. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "assigned": 1024, 
  "activated": 1024,
  "sharedComputerActivation": 1024
}
```


