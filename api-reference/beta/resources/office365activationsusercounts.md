---
title: Тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 90d9d2d8616f166eb9d8b87967898daa0468db54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081406"
---
# <a name="office365activationsusercounts-resource-type"></a>Тип ресурса office365ActivationsUserCounts

## <a name="properties"></a>Свойства

| Свойство                 | Тип   | Description                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | Date   | Последняя дата контента.          |
| productType              | String | Тип продукта, например «Office 365 профессиональный плюс», «Клиент Project», или «Visio Pro для Office 365". |
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
