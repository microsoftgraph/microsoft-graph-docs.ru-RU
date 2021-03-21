---
title: removeContentHeaderAction resource type
description: Представляет действие, которое указывает сведения о загонах контента, которые будут удалены из сведений, если это применимо.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 9170556f5fc04e7b270d9886cd81f48c45e07122
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962084"
---
# <a name="removecontentheaderaction-resource-type"></a>removeContentHeaderAction resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, которое указывает сведения о загонах контента, которые будут удалены из сведений, если это применимо. [ОценкаApplication,](../api/informationprotectionlabel-evaluateapplication.md) [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)или оценка APIRemoval могут возвращать **удалениеContentHeaderAction,** если заголовок должен быть удален в результате обновления или удаления метки. [](../api/informationprotectionlabel-evaluateremoval.md) Действие предписывает потребляемому приложению удалить определенный элемент пользовательского интерфейса, содержащий ранее применимый заголовок контента.

## <a name="properties"></a>Свойства

| Свойство       | Тип              | Описание                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| uiElementNames | Коллекция строк | Имя элемента пользовательского интерфейса удаляемого заголовщика. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeContentHeaderAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "uiElementNames": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "removeContentHeaderAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

