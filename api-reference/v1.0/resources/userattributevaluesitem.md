---
title: тип ресурса userAttributeValuesItem
description: Представляет значения атрибута потока пользователей в потоке пользователей.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 690b9f53762359ab559fb98534525cad15e5e282
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59083966"
---
# <a name="userattributevaluesitem-resource-type"></a>тип ресурса userAttributeValuesItem

Пространство имен: microsoft.graph

Представляет значения атрибута потока пользователей в потоке пользователей, если необходимо выбрать несколько выборов.  UserAttributeValuesItem применим к userInputTypes , и для `radioSingleSelect` `dropdownSingleSelect` `checkboxMultiSelect` [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|isDefault|Boolean|Определяет, установлено ли значение по умолчанию.|
|name|String|Отображает имя свойства, отображаемого пользователю в потоке пользователей.|
|value|String|Значение, заданной при выборе этого элемента.|

## <a name="relationships"></a>Отношения

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
