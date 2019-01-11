---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 25812d48626c7dc5e468915f7308941a4f74b38e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860965"
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

