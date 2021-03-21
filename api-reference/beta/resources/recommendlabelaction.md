---
title: recommendLabelAction resource type
description: Представляет метку, которую следует рекомендовать пользователю для приложения к файлу на основе типов конфиденциальной информации.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 10d3ac687605ab648cdd3d68d6a3721c8fba2e30
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962576"
---
# <a name="recommendlabelaction-resource-type"></a>recommendLabelAction resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет метку, которую следует рекомендовать пользователю для приложения к файлу на основе обнаруженных типов конфиденциальной информации. В [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) может быть возвращена **рекомендацияLabelAction,** если политика  маркировки Microsoft Information Protection настроена на рекомендации и метку, а не на принудительное выполнение метки. Пользователь или прикладный пользователь может игнорировать или принимать эту рекомендацию. 

## <a name="properties"></a>Свойства

| Свойство                    | Тип                                                                     | Описание                                                           |
| :-------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| actionSource                | String                                                                   | Возможные значения: `manual`, `automatic`, `recommended`, `default`. |
| actions                     | [коллекция informationProtectionAction](informationprotectionaction.md) | Действия, которые необходимо принять, если метка принята пользователем.                                                                       |
| label                       | [labelDetails](labeldetails.md)                                          | Метка, которая рекомендуется.                                                                      |
| responsibleSensitiveTypeIds | Коллекция объектов Guid                                                          | GUID типа конфиденциальной информации, из-за чего была дана рекомендация.                                                                      |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recommendLabelAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "actionSource": "String",
  "actions": [{"@odata.type": "microsoft.graph.informationProtectionAction"}],
  "label": {"@odata.type": "microsoft.graph.labelDetails"},
  "responsibleSensitiveTypeIds": ["Guid"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recommendLabelAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


