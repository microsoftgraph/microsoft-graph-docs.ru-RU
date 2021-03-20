---
title: тип ресурса applyLabelAction
description: Представляет набор действий, которые необходимо принять для применения или обновления метки.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e53a2796c7cd4f0b8c0a415ca4bc38ffefeb609e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945744"
---
# <a name="applylabelaction-resource-type"></a>тип ресурса applyLabelAction

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет набор действий, которые необходимо принять для применения или обновления метки. **applyLabelAction** возвращается, когда результатом операции оценки меток является применение метки. Свойство `actions` содержит [коллекцию informationProtectionAction,](informationProtectionaction.md) в которую описан  полный набор действий для применения метки, включая удаление старых метаданных, маркировку контента и защиту.

## <a name="properties"></a>Свойства

| Свойство                    | Тип                                                                     | Описание                                                                                                                                                                                       |
| :-------------------------- | :----------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| actionSource                | String                                                                   | Возможные значения: `manual`, `automatic`, `recommended`, `default`.                                                                                                                             |
| actions                     | [коллекция informationProtectionAction](informationprotectionaction.md) | Коллекция определенных действий, которые должно приниматься потреблять приложение для метки документа. Полный список см. в списке [informationProtectionAction.](informationprotectionaction.md) |
| label                       | [labelDetails](labeldetails.md)                                          | Объект, описывая детали метки для применения.                                                                                                                                          |
| responsibleSensitiveTypeIds | Коллекция объектов Guid                                                          | Если метка была результатом автоматической классификации, введите список GUID-интерфейсов типа конфиденциальной информации, которые привели к возврату метки.                                         
## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applyLabelAction",
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
  "description": "applyLabelAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

