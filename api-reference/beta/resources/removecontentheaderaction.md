---
title: Тип ресурса Ремовеконтенсеадерактион
description: Представляет действие, задающее сведения о заголовке контента, которые необходимо удалить из информации (если это возможно).
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 99f3b77607b34cb68cdef3fa9fc5658ed06b52ec
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938943"
---
# <a name="removecontentheaderaction-resource-type"></a>Тип ресурса Ремовеконтенсеадерактион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие, задающее сведения о заголовке контента, которые необходимо удалить из информации (если это возможно). API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md) могут возвращать **ремовеконтенсеадерактион** , если заголовок будет удален в результате обновления или удаления метки. Действие предписывает приложению, которое использует приложение, удалить определенный элемент пользовательского интерфейса, который содержит заданный ранее заголовок контента.

## <a name="properties"></a>Свойства

| Свойство       | Тип              | Описание                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| уиелементнамес | Коллекция строк | Имя элемента пользовательского интерфейса заголовка, который требуется удалить. |

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