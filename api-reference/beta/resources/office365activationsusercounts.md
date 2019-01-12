---
title: Тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3dc497e516f95f1e05167703f2b9f8aea6363a64
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917722"
---
# <a name="office365activationsusercounts-resource-type"></a>Тип ресурса office365ActivationsUserCounts

## <a name="properties"></a>Свойства

| Свойство                 | Тип   | Описание                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Date   | Последняя дата контента.          |
| productType              | Строка | Тип продукта, например «Office 365 профессиональный плюс», «Клиент Project», или «Visio Pro для Office 365". |
| назначенные                 | Int64  | Число пользователей, которым был назначен для лицензии. |
| активирован                | Int64  | Количество пользователей, активации продукта. |
| sharedComputerActivation | Int64  | Количество пользователей, которые используются продукта на совместно используемый компьютер. |

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
