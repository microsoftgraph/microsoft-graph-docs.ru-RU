---
title: Тип ресурса userAttributeValuesItem
description: Используется для заполнения значений атрибута пользовательского потока в пользовательском потоке при выборе нескольких вариантов.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 64b2416cd6fd0e8c92d9a00ff2d599226e3cd02c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133023"
---
# <a name="userattributevaluesitem-resource-type"></a>Тип ресурса userAttributeValuesItem

Пространство имен: microsoft.graph

Используется для заполнения значений атрибута пользовательского потока в пользовательском потоке при выборе нескольких вариантов. userAttributeValuesItem применимо к userInputTypes , и `radioSingleSelect` `dropdownSingleSelect` для `checkboxMultiSelect` [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|isDefault|Boolean|Используется для настройки значения по умолчанию.|
|name|String|Отображаемого имени свойства, отображаемого для конечного пользователя в пользовательском потоке.|
|value|String|Значение, заданной при выборе этого элемента.|

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
