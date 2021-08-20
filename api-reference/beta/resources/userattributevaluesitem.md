---
title: тип ресурса userAttributeValuesItem
description: Используется для заполнения значений атрибута потока пользователей в потоке пользователей при выборе нескольких выборов.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1780e37b8be9952d314f2a95a89975814ffac3483199ae72eb608d1426aa84cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145077"
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
