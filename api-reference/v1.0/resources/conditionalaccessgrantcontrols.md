---
title: Тип ресурса Кондитионалакцессгрантконтролс
description: Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e48d179e53111cc69b72eb8aa61c52ae105764df
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018909"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a>Тип ресурса Кондитионалакцессгрантконтролс

Пространство имен: microsoft.graph

Представляет элементы управления предоставлением, которые должны быть выполнены для передачи политики.

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:-------- |:---- |:----------- |
| operator | String | Определяет связь элементов управления предоставлением. Возможные значения: `AND` , `OR` . |
| буилтинконтролс | Коллекция String | Список значений встроенных элементов управления, необходимых для политики. Возможные значения: `Block` , `Mfa` , `CompliantDevice` , `DomainJoinedDevice` , `ApprovedApplication` , `CompliantApplication` |
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

