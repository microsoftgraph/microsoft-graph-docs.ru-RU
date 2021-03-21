---
title: removeProtectionAction resource type
description: Представляет действие по удалению защиты из файла или сведений.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2b315c9d2641524d8a134f0e0b9704c51419ada4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962037"
---
# <a name="removeprotectionaction-resource-type"></a>removeProtectionAction resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет действие по удалению защиты из файла или сведений. [ОценкаApplication,](../api/informationprotectionlabel-evaluateapplication.md) [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)или оценка APIRemoval могут вернуть **removeProtectionAction,** если защита будет удалена в результате обновления или удаления метки. [](../api/informationprotectionlabel-evaluateremoval.md) Действие предписывает потребляемому приложению удалить определенный элемент пользовательского интерфейса, содержащий ранее применимый заголовок контента. Защита должна быть удалена с помощью клиентской библиотеки, например SDK Microsoft Information Protection, только если у вызываемого пользователя достаточно прав для удаления защиты.

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

