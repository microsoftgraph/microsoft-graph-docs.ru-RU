---
title: Тип ресурса Апплилабелактион
description: Представляет набор действий, которые следует предпринять для применения или обновления метки.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fc7911b3a225f226edc74dc9b194a2522b7c4251
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939147"
---
# <a name="applylabelaction-resource-type"></a>Тип ресурса Апплилабелактион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет набор действий, которые следует предпринять для применения или обновления метки. **апплилабелактион** возвращается, когда результат операции оценки метки состоит в том, что метка должна быть применена. Свойство содержит коллекцию [информатионпротектионактион](informationProtectionaction.md) , в которой описывается полный набор действий для применения метки, включая удаление старых метаданных, маркировки содержимого и защиту. ** `actions`

## <a name="properties"></a>Свойства

| Свойство                    | Тип                                                                     | Описание                                                                                                                                                                                       |
| :-------------------------- | :----------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| актионсаурце                | String                                                                   | Возможные значения: `manual`, `automatic`, `recommended`, `default`.                                                                                                                             |
| actions                     | Коллекция [информатионпротектионактион](informationprotectionaction.md) | Коллекция определенных действий, которые будут выполняться приложением использования для добавления метки в документ. Полный список представлен в [информатионпротектионактион](informationprotectionaction.md) . |
| label                       | [лабелдетаилс](labeldetails.md)                                          | Объект, описывающий сведения о применяемой метке.                                                                                                                                          |
| респонсиблесенситиветипеидс | Коллекция объектов Guid                                                          | Если метка была результатом автоматической классификации, предоставьте список идентификаторов GUID типа конфиденциальной информации, которые привели к возвращенной метке.                                         
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