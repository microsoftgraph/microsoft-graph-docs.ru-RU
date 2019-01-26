---
title: Тип ресурса office365ActivationsUserCounts
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0d5ed2af02f429f5fd4d6e92b408d2e8e420f4d0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574546"
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
