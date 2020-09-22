---
title: Тип ресурса Ремовепротектионактион
description: Представляет действие для удаления защиты из файла или информации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bf4ad367038367d3572f0451bfa7d3eb0a25368d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073399"
---
# <a name="removeprotectionaction-resource-type"></a>Тип ресурса Ремовепротектионактион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие для удаления защиты из файла или информации. API [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md), [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md)или [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md) могут возвращать **ремовепротектионактион** , если необходимо удалить защиту в результате обновления или удаления метки. Действие предписывает приложению, которое использует приложение, удалить определенный элемент пользовательского интерфейса, который содержит заданный ранее заголовок контента. Защита должна быть удалена с помощью клиентской библиотеки, например Microsoft Information Protection SDK, только в том случае, если вызывающий пользователь имеет достаточные права на удаление защиты.

## <a name="properties"></a>Свойства

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeProtectionAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "removeProtectionAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

