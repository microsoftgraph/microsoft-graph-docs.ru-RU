---
title: тип ресурса informationProtectionLabel
description: Описывает метку защиты информации, которая описывает, как правильно применять метку конфиденциальности к сведениям.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ee8865b4fa898a91ca79cfba29c928ed00e21ae2
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579671"
---
# <a name="informationprotectionlabel-resource-type"></a>тип ресурса informationProtectionLabel

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает метку защиты информации, которая описывает, как правильно применять метку конфиденциальности к сведениям. Ресурс **informationProtectionLabel** описывает конфигурацию меток конфиденциальности, которые применяются к пользователю или клиенту.  

## <a name="methods"></a>Методы

| Метод                                                                                              | Возвращаемый тип                                                               | Описание                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [List informationProtectionLabel](../api/informationprotectionpolicy-list-labels.md)                | [коллекция informationProtectionLabel](informationprotectionlabel.md) | Список всех настроенных меток защиты информации для пользователя или клиента.                                                                                                |
| [Получить informationProtectionLabel](../api/informationprotectionlabel-get.md)                          | [informationProtectionLabel](informationprotectionlabel.md)               | Учитывая определенный ID метки, **верните informationProtectionLabel**.                                                                                                  |
| [evaluateapplication](../api/informationprotectionlabel-evaluateapplication.md)                     | [коллекция informationProtectionAction](informationprotectionaction.md)  | Учитывая вход [контентаInfo](contentinfo.md) и [labelingOptions,](labelingoptions.md)вычислить набор действий, необходимых для применения метки.                      |
| [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) | [коллекция informationProtectionAction](informationprotectionaction.md)  | Учитывая ввод [контентаInfo и](contentinfo.md) результаты классификации, вычислить набор действий, необходимых для применения метки.                                  |
| [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)                             | [коллекция informationProtectionAction](informationprotectionaction.md)  | Учитывая вход [контентаInfo](contentinfo.md) и [downgradeJustification,](downgradejustification.md)вычислять действия, которые необходимо принять для удаления метки. |
| [extractLabel](../api/informationprotectionlabel-extractlabel.md)                                   | [informationProtectionContentLabel](informationprotectioncontentlabel.md) | Учитывая вход [контентаInfo,](contentinfo.md)возвращайте сведения о [informationProtectionLabel,](informationprotectionlabel.md) который представляют метаданные.       |

## <a name="properties"></a>Свойства

| Свойство    | Тип    | Описание                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| color       | String  | Цвет, который должен отображаться пользовательским интерфейсом для метки, если настроен.                              |
| description | Строка  | Описание метки, определенное администратором.                                                    |
| id          | Строка  | Идентификатор метки — это уникальный идентификатор глобального масштаба (GUID)                                             |
| isActive    | Boolean | Указывает, активна метка или нет. Активные метки должны быть скрыты или отключены в пользовательском интерфейсе. |
| name        | String  | Простое имя метки.                                                                |
| sensitivity | Int32   | Значение чувствительности метки, где более низкий уровень менее чувствителен.                              |
| tooltip     | Строка  | Инструмент, который должен отображаться для метки в пользовательском интерфейсе.                                     |
| родитель      | labelDetails   | Родительская метка, связанная с детской меткой. Null, если метка не имеет родительского знака.

## <a name="relationships"></a>Отношения

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
  "tooltip": "String",
  "parent": {"@odata.type": "microsoft.graph.labelDetails" }
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


