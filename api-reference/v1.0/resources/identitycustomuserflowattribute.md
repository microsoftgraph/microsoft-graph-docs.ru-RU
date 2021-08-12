---
title: тип ресурса identityCustomUserFlowAttribute
description: Представляет настраиваемый атрибут потока пользователей в Azure Active Directory клиентах, который можно использовать в потоке пользователей самообслуживки.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5fdad3bf3fabb75cfa882e2c9b78dd2f008a596e70630b5eb34b3f3aa215baff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126580"
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

## <a name="relationships"></a>Связи

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
