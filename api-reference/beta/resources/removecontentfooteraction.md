---
title: Тип ресурса Ремовеконтентфутерактион
description: Представляет действие, задающее сведения о нижнем колонтитуле контента, который необходимо удалить из информации, если это возможно.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 76450b0d6b0f3a532a4e3472d2ce99ead8c933e4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073455"
---
# <a name="removecontentfooteraction-resource-type"></a>Тип ресурса Ремовеконтентфутерактион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, задающее сведения о нижнем колонтитуле контента, который необходимо удалить из информации, если это возможно. API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateApplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md) могут возвращать **ремовеконтентфутерактион** , если нижний колонтитул необходимо удалить в результате обновления или удаления метки. Действие предписывает приложению, которое использует приложение, удалить определенный элемент пользовательского интерфейса, содержащий ранее соответствующий нижний колонтитул контента.

## <a name="properties"></a>Свойства

| Свойство       | Тип              | Описание                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| уиелементнамес | Коллекция String | Имя элемента пользовательского интерфейса нижнего колонтитула, который требуется удалить. |

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

