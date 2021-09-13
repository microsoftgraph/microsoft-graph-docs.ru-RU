---
title: тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: c566383e339b4277b93fcd5177068f179626a570
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033296"
---
# <a name="office365activationsusercounts-resource-type"></a>тип ресурса office365ActivationsUserCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство                 | Тип   | Описание                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Дата   | Последняя дата контента.          |
| productType              | String | Тип продукта, например "Microsoft 365 ProPlus" или "Project клиент". |
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


