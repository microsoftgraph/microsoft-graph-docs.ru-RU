---
title: Тип ресурса recommendLabelAction
description: Представляет метку, которая должна быть рекомендована пользователю для приложения к файлу на основе типов конфиденциальной информации.
ms.localizationpriority: medium
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 245aae5c65d08d5a1755434917afe9b22f4c43b2
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883840"
---
# <a name="recommendlabelaction-resource-type"></a>Тип ресурса recommendLabelAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет метку, которая должна быть рекомендована пользователю для приложения к файлу на основе обнаруженных типов конфиденциальной информации. [Объект evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) может возвращать **recommendLabelAction**, если в политике меток Microsoft Purview Information Protection задано значение **recommend** и label, а не принудительное применение метки. Пользователь или приложение могут игнорировать или принимать рекомендацию. 

## <a name="properties"></a>Свойства

| Свойство                    | Тип                                                                     | Описание                                                           |
| :-------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| actionSource                | String                                                                   | Возможные значения: `manual`, `automatic`, `recommended`, `default`. |
| actions                     | [Коллекция informationProtectionAction](informationprotectionaction.md) | Действия, выполняемые, если метка принимается пользователем.                                                                       |
| label                       | [labelDetails](labeldetails.md)                                          | Рекомендуемая метка.                                                                      |
| responsibleSensitiveTypeIds | Коллекция объектов Guid                                                          | Идентификаторы GUID типа конфиденциальной информации, которые вызвали рекомендацию.                                                                      |

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


