---
title: тип ресурса userAttributeValuesItem
description: Представляет значения атрибута потока пользователей в потоке пользователей.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 88e19bfa02876e08df4c3040ff6bcfefae41840278719b83ccc7b57be651f5a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205215"
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
