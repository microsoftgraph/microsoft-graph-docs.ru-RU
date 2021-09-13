---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 47c3fbe839b5e5f17e76217ca2cda633d8c42c6a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134138"
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
| id  | string | Идентификатор сеанса книги. |
| persistChanges | boolean |  Имеет значение `true` для сохраняемого сеанса. Имеет значение `false` для несохраняемого сеанса (режим просмотра) |


