---
title: Тип ресурса Рекоммендлабелактион
description: Представляет метку, которая должна быть рекомендована пользователю для приложения в файл на основе типов конфиденциальной информации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54f2a872c0aa64eb79e0b8755ddc6b3788f14055
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939378"
---
# <a name="recommendlabelaction-resource-type"></a>Тип ресурса Рекоммендлабелактион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет метку, которая должна быть рекомендована пользователю для приложения в файл на основе обнаруженных типов конфиденциальной информации. [Евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateClassificationResults.md) может возвращать **рекоммендлабелактион** , если для политики метки Microsoft Information Protection задано значение **рекомендовать** и подпись, а не задано применение метки. Пользователь или апплиатион может игнорировать или принять рекомендацию. 

## <a name="properties"></a>Свойства

| Свойство                    | Тип                                                                     | Описание                                                           |
| :-------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| актионсаурце                | String                                                                   | Возможные значения: `manual`, `automatic`, `recommended`, `default`. |
| actions                     | Коллекция [информатионпротектионактион](informationprotectionaction.md) | Действия, которые необходимо выполнить, если пользователь принимает метку.                                                                       |
| label                       | [лабелдетаилс](labeldetails.md)                                          | Рекомендуемая метка.                                                                      |
| респонсиблесенситиветипеидс | Коллекция объектов Guid                                                          | Идентификаторы GUID типа конфиденциальной информации, которые привели к выдано рекомендация.                                                                      |

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
