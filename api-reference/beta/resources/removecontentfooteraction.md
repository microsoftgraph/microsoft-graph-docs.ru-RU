---
title: removeContentFooterAction resource type
description: Представляет действие, которое указывает сведения на подножке контента, которые будут удалены из сведений, если это применимо.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1e8de130b2ad346e8e1fee2077014eda9e9b94d5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962093"
---
# <a name="removecontentfooteraction-resource-type"></a>removeContentFooterAction resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, которое указывает сведения на подножке контента, которые будут удалены из сведений, если это применимо. [ОценкаApplication,](../api/informationprotectionlabel-evaluateApplication.md) [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)или оценка APIRemoval могут возвращать **removeContentFooterAction,** если в результате обновления или удаления метки необходимо удалить подножку. [](../api/informationprotectionlabel-evaluateremoval.md) Действие предписывает потребляемому приложению удалить определенный элемент пользовательского интерфейса, содержащий ранее применимый подножок контента.

## <a name="properties"></a>Свойства

| Свойство       | Тип              | Описание                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| uiElementNames | Коллекция строк | Имя элемента пользовательского интерфейса необходимо удалить. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeContentFooterAction",
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
  "description": "removeContentFooterAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

