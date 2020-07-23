---
title: Тип ресурса Кондитионалакцессгрантконтролс
description: Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aadf38ac5cff15e4c085f77df36aa6fd48fa272f
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384684"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a>Тип ресурса Кондитионалакцессгрантконтролс

Пространство имен: microsoft.graph

Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| operator | String | Определяет связь элементов управления предоставлением. Возможные значения: `AND` , `OR` . |
| буилтинконтролс | Коллекция String | Список значений встроенных элементов управления, необходимых для политики. Возможные значения: `Block` , `Mfa` , `CompliantDevice` , `DomainJoinedDevice` , `ApprovedApplication` ,`CompliantApplication` |
| кустомаусентикатионфакторс | Коллекция String | Список идентификаторов настраиваемых элементов управления, необходимых для политики. Более подробную информацию можно узнать в статье [настраиваемые элементы управления](https://docs.microsoft.com/azure/active-directory/conditional-access/controls). |
| термсофусе | Коллекция String | Список [условий использования](https://docs.microsoft.com/graph/api/resources/agreement) идентификаторов, необходимых для политики. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "operator",
    "builtInControls",
    "customAuthenticationFactors",
    "termsOfUse"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessGrantControls",
  "baseType": null
}-->

```json
{
  "builtInControls": ["String"],
  "customAuthenticationFactors": ["String"],
  "operator": "String",
  "termsOfUse": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessGrantControls resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
