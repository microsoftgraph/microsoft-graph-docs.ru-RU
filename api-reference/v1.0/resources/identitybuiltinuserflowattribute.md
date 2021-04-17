---
title: identityBuiltInUserFlowAttribute type
description: Представляет встроенный атрибут потока пользователей в клиентах Azure Active Directory, который можно использовать в потоке пользователей для самостоятельной регистрации.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c549be6035b26d6e2d7faedafb6848240a9303dc
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883346"
---
# <a name="identitybuiltinuserflowattribute-resource-type"></a>identityBuiltInUserFlowAttribute type

Пространство имен: microsoft.graph

Представляет встроенный атрибут потока пользователей в клиентах Azure Active Directory, который можно использовать в потоке пользователей для самостоятельной регистрации. Эти атрибуты не могут быть изменены и являются только для чтения.

Наследует [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор атрибута потока пользователей. Это автоматически созданный атрибут только для чтения. Унаследованный от [identityUserFlowAttribute](../resources/identityuserflowattribute.md)|
|displayName|String|Отображаемое имя атрибута потока пользователей. Наследуется [от identityUserFlowAttribute](../resources/identityuserflowattribute.md). Только для чтения.|
|description|String|Описание атрибута потока пользователей, демонстрируемое пользователю при регистрации. Наследуется [от identityUserFlowAttribute](../resources/identityuserflowattribute.md). Только для чтения.|
|userFlowAttributeType|identityUserFlowAttributeType|Тип атрибута потока пользователей. Это автоматически настроенный атрибут только для чтения. Значение для этого свойства будет `builtIn` . Наследуется [от identityUserFlowAttribute](../resources/identityuserflowattribute.md). Только для чтения.|
|dataType|identityUserFlowAttributeDataType|Тип данных атрибута потока пользователей. Это свойство нельзя изменить после создания атрибута потока пользователей. Поддерживаемые значения для **dataType**: `string`, `boolean`, `int64`, `stringCollection`, `dateTime`. Наследуется [от identityUserFlowAttribute](../resources/identityuserflowattribute.md). Только для чтения.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityBuiltInUserFlowAttribute",
  "baseType": "microsoft.graph.identityUserFlowAttribute",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityBuiltInUserFlowAttribute",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "userFlowAttributeType": "String",
  "dataType": "String"
}
```
