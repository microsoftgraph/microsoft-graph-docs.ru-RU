---
title: тип ресурса identityCustomUserFlowAttribute
description: Представляет настраиваемый атрибут потока пользователей в Azure Active Directory клиентах, который можно использовать в потоке пользователей самообслуживки.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 592a350b03f282900cc4badbe7e5c2e1179e58a5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59056076"
---
# <a name="identitycustomuserflowattribute-resource-type"></a>тип ресурса identityCustomUserFlowAttribute

Пространство имен: microsoft.graph

Представляет настраиваемый атрибут потока пользователей в Azure Active Directory клиентах, который можно использовать в потоке пользователей самообслуживки. Эти атрибуты не могут быть изменены и являются только для чтения.

Наследует [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор атрибута потока пользователей. Это автоматически созданный атрибут только для чтения. Унаследованный от [identityUserFlowAttribute](../resources/identityuserflowattribute.md)|
|displayName|String|Отображаемое имя атрибута потока пользователей. Унаследованный от [identityUserFlowAttribute](../resources/identityuserflowattribute.md)|
|description|String|Описание атрибута потока пользователей, демонстрируемое пользователю при регистрации. Унаследованный от [identityUserFlowAttribute](../resources/identityuserflowattribute.md)|
|userFlowAttributeType|identityUserFlowAttributeType|Тип атрибута потока пользователей. Это автоматически настроенный атрибут только для чтения. Значение для этого свойства будет `custom` . Наследуется [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).|
|dataType|identityUserFlowAttributeDataType|Тип данных атрибута потока пользователей. Это свойство нельзя изменить после создания атрибута потока пользователей. Поддерживаемые значения для **dataType**: `string`, `boolean`, `int64`, `stringCollection`, `dateTime`. Наследуется [от identityUserFlowAttribute](../resources/identityuserflowattribute.md).|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityCustomUserFlowAttribute",
  "baseType": "microsoft.graph.identityUserFlowAttribute",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityCustomUserFlowAttribute",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "userFlowAttributeType": "String",
  "dataType": "String"
}
```
