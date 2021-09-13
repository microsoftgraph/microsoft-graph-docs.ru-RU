---
title: тип ресурса userAttributeValuesItem
description: Используется для заполнения значений атрибута потока пользователей в потоке пользователей при выборе нескольких выборов.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3468ed1545c8be12f906182f34f5260897f461ba
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057000"
---
# <a name="userattributevaluesitem-resource-type"></a>тип ресурса userAttributeValuesItem

Пространство имен: microsoft.graph

Используется для заполнения значений атрибута потока пользователей в потоке пользователей при выборе нескольких выборов. userAttributeValuesItem применим к userInputTypes , и для `radioSingleSelect` `dropdownSingleSelect` `checkboxMultiSelect` [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|isDefault|Boolean|Используется для настройки значения по умолчанию.|
|name|String|Отображает имя свойства, отображаемого конечному пользователю в потоке пользователей.|
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
