---
title: Тип ресурса Информатионпротектионлабел
description: Описывает метку Information Protection, которая подробно описывает, как правильно применять метку конфиденциальности к данным.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 183a5856aafd8aa2a5b8b1fe3b1eb48bddcc5358
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496042"
---
# <a name="informationprotectionlabel-resource-type"></a>Тип ресурса Информатионпротектионлабел

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает метку Information Protection, которая подробно описывает, как правильно применять метку конфиденциальности к данным. Ресурс **информатионпротектионлабел** описывает конфигурацию меток конфиденциальности, которые применяются к пользователю или клиенту.  

## <a name="methods"></a>Методы

| Метод                                                                                              | Возвращаемый тип                                                               | Описание                                                                                                                                                            |
| :-------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [Список Информатионпротектионлабел](../api/informationprotectionpolicy-list-labels.md)                | Коллекция [информатионпротектионлабел](informationprotectionlabel.md) | Перечисление всех настроенных меток защиты информации для пользователя или клиента.                                                                                                |
| [Получение Информатионпротектионлабел](../api/informationprotectionlabel-get.md)                          | [информатионпротектионлабел](informationprotectionlabel.md)               | При наличии определенного идентификатора метки возвратите **информатионпротектионлабел**.                                                                                                  |
| [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md)                     | Коллекция [информатионпротектионактион](informationprotectionaction.md)  | При наличии входных данных для [контентинфо](contentinfo.md) и [лабелингоптионс](labelingoptions.md)расчет набора действий требует применения метки.                      |
| [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md) | Коллекция [информатионпротектионактион](informationprotectionaction.md)  | Имея входные данные о [контентинфо](contentinfo.md) и классификации, вычислите набор действий, необходимых для применения метки.                                  |
| [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md)                             | Коллекция [информатионпротектионактион](informationprotectionaction.md)  | При наличии входных данных для [контентинфо](contentinfo.md) и [довнградежустификатион](downgradejustification.md)вычисляет действия, которые следует предпринять для удаления метки. |
| [екстрактлабел](../api/informationprotectionlabel-extractlabel.md)                                   | [информатионпротектионконтентлабел](informationprotectioncontentlabel.md) | При наличии входных данных [контентинфо](contentinfo.md)возвращает сведения о [информатионпротектионлабел](informationprotectionlabel.md) , которые представляют метаданные.       |

## <a name="properties"></a>Свойства

| Свойство    | Тип    | Описание                                                                                     |
| :---------- | :------ | :---------------------------------------------------------------------------------------------- |
| color       | String  | Цвет, который должен отображаться в пользовательском интерфейсе для метки, если она настроена.                              |
| description | String  | Заданное администратором описание метки.                                                    |
| id          | Строка  | ИДЕНТИФИКАТОР метки является глобальным уникальным идентификатором (GUID)                                             |
| isActive    | Логический | Указывает, активна ли метка. Активные метки должны быть скрыты или отключены в пользовательском интерфейсе. |
| name        | String  | Имя в виде открытого текста метки.                                                                |
| sensitivity | Int32   | Значение чувствительности метки, где меньше конфиденциально.                              |
| tooltip     | String  | Всплывающая подсказка, отображаемая для метки в пользовательском интерфейсе.                                     |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationProtectionLabel",
  "baseType": "",
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
