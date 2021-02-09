---
title: Тип ресурса informationProtectionLabel
description: Описание метки защиты информации, которая описывает, как правильно применить метку конфиденциальности к информации.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 694015f819d1c1afc9fe9feb23c67c92c05eed70
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153636"
---
# <a name="informationprotectionlabel-resource-type"></a>Тип ресурса informationProtectionLabel

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описание метки защиты информации, которая описывает, как правильно применить метку конфиденциальности к информации. Ресурс **informationProtectionLabel** описывает конфигурацию меток конфиденциальности, которые применяются к пользователю или арендатору.  

## <a name="methods"></a>Методы

| Метод                                                                                              | Возвращаемый тип                                                               | Описание                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Список informationProtectionLabel](../api/informationprotectionpolicy-list-labels.md)                | [Коллекция informationProtectionLabel](informationprotectionlabel.md) | Список всех настроенных меток защиты информации для пользователя или клиента.                                                                                                |
| [Get informationProtectionLabel](../api/informationprotectionlabel-get.md)                          | [informationProtectionLabel](informationprotectionlabel.md)               | С учетом определенного ИД метки **вернете informationProtectionLabel.**                                                                                                  |
| [evaluateapplication](../api/informationprotectionlabel-evaluateapplication.md)                     | [Коллекция informationProtectionAction](informationprotectionaction.md)  | Учитывая входные данные [contentInfo](contentinfo.md) и [labelingOptions,](labelingoptions.md)вычислите набор действий, необходимых для применения метки.                      |
| [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) | [Коллекция informationProtectionAction](informationprotectionaction.md)  | С учетом [входных данных contentInfo](contentinfo.md) и результатов классификации вычислить набор действий, необходимых для применения метки.                                  |
| [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)                             | [Коллекция informationProtectionAction](informationprotectionaction.md)  | Учитывая входные данные [contentInfo](contentinfo.md) и [downgradeJustification,](downgradejustification.md)вычислите действия, которые необходимо принять для удаления метки. |
| [extractLabel](../api/informationprotectionlabel-extractlabel.md)                                   | [informationProtectionContentLabel](informationprotectioncontentlabel.md) | При вводе [contentInfo](contentinfo.md)возвращает сведения о [метке informationProtectionLabel,](informationprotectionlabel.md) которую представляют метаданные.       |

## <a name="properties"></a>Свойства

| Свойство    | Тип    | Описание                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| color       | String  | Цвет, который должен отображаться в пользовательском интерфейсе для метки, если он настроен.                              |
| description | String  | Описание метки, определенное администратором.                                                    |
| id          | String  | Идентификатор метки — это глобальный уникальный идентификатор (GUID)                                             |
| isActive    | Boolean | Указывает, активна ли метка. Активные метки должны быть скрыты или отключены в пользовательском интерфейсе. |
| name        | String  | Обычное имя метки.                                                                |
| sensitivity | Int32   | Значение конфиденциальности метки, где меньшее значение менее конфиденциально.                              |
| tooltip     | String  | The tooltip that should be displayed for the label in a UI.                                     |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationProtectionLabel",
  "keyProperty": "id"
}-->

```json
{
  "color": "String",
  "description": "String",
  "id": "String (identifier)",
  "isActive": true,
  "name": "String",
  "sensitivity": 1024,
  "tooltip": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


