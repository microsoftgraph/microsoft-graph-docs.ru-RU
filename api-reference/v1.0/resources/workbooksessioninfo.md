---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f2e6b925e7cc1790b1c6d4f08bab02fa92f19936
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033336"
---
# <a name="workbooksessioninfo-resource-type"></a>Тип ресурса workbookSessionInfo

Предоставляет сведения о сеансе книги.


## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a>Свойства

| Свойство | Тип  | Описание                               |
|:---------|:------|:------------------------------------------|
| id  | string | Идентификатор сеанса книги. |
| persistChanges | boolean |  Имеет значение `true` для сохраняемого сеанса. Имеет значение `false` для несохраняемого сеанса (режим просмотра) |

