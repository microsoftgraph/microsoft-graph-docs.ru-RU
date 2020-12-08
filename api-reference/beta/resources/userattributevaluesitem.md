---
title: Тип ресурса Усераттрибутевалуеситем
description: Используется для заполнения значений атрибута Flow Flow в пользовательском цикле, если выбрано несколько вариантов.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6fd0d582ef4dcdd83dba6947536c5acdbc14a8cb
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581419"
---
# <a name="userattributevaluesitem-resource-type"></a>Тип ресурса Усераттрибутевалуеситем

Пространство имен: microsoft.graph

Используется для заполнения значений атрибута Flow Flow в пользовательском цикле, если выбрано несколько вариантов. Усераттрибутевалуеситем применяется к Усеринпуттипес `radioSingleSelect` , `dropdownSingleSelect` и `checkboxMultiSelect` для [идентитюсерфловаттрибутеассигнмент](..\resources\identityuserflowattributeassignment.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|isDefault|Boolean|Используется, чтобы задать значение по умолчанию.|
|name|String|Отображаемое имя свойства, отображаемого для конечного пользователя в пользовательском движении.|
|value|String|Значение, заданное при выборе этого элемента.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userAttributeValuesItem"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userAttributeValuesItem",
  "name": "String",
  "value": "String",
  "isDefault": "Boolean"
}
```
