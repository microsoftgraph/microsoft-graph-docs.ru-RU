---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
ms.openlocfilehash: 5a86fd4dfd653f16445eeccad8478db56db0ac5f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316844"
---
# <a name="workbooksessioninfo-resource-type"></a>Тип ресурса workbookSessionInfo

Предоставляет сведения о сеансе книги.


## <a name="json-representation"></a>Представление в формате JSON

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
| id  | строка | Идентификатор сеанса книги. |
| persistChanges | строка |  Имеет значение `true` для сохраняемого сеанса. Имеет значение `false` для несохраняемого сеанса (режим просмотра) |

