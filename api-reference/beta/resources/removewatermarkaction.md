---
title: removeWatermarkAction resource type
description: Представляет действие, которое указывает сведения о водяном знаке контента, который должен быть удален из сведений, если это применимо.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2a2365b2c9bc1080db9b6bf58b2035d88832881a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960357"
---
# <a name="removewatermarkaction-resource-type"></a>removeWatermarkAction resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, которое указывает сведения о водяном знаке контента, который должен быть удален из сведений, если это применимо. [ОценкаApplication,](../api/informationprotectionlabel-evaluateapplication.md) [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)или оценка APIRemoval могут возвращать **removeWatermarkAction,** если водяной знак будет удален в результате обновления или удаления метки. [](../api/informationprotectionlabel-evaluateremoval.md) Действие предписывает потребляемому приложению удалить определенный элемент пользовательского интерфейса, содержащий ранее применимый водяной знак контента.

## <a name="properties"></a>Свойства

| Свойство       | Тип              | Описание                           |
| :------------- | :---------------- | :------------------------------------ |
| uiElementNames | Коллекция строк | Имя элемента пользовательского интерфейса подножки, который следует удалить. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeWatermarkAction",
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
  "description": "removeWatermarkAction resource",
  "keywords": "",  
  "section": "documentation",
  "tocPath": ""
}-->

