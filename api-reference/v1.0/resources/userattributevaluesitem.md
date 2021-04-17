---
title: тип ресурса userAttributeValuesItem
description: Представляет значения атрибута потока пользователей в потоке пользователей.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 367f5d835f3790c589a8d7d28b7994484fd9613c
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882450"
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
