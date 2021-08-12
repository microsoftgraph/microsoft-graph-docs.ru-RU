---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8957acbfa1ed8eaff40fd5799471aff67bdd77bf634f9febeef9dbc7677e6589
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196455"
---
# <a name="workbooksessioninfo-resource-type"></a>Тип ресурса workbookSessionInfo

Пространство имен: microsoft.graph

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
| id  | строка | Идентификатор сеанса книги. |
| persistChanges | логический |  Имеет значение `true` для сохраняемого сеанса. Имеет значение `false` для несохраняемого сеанса (режим просмотра) |


