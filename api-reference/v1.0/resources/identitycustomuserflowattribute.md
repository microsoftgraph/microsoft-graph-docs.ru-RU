---
title: тип ресурса identityCustomUserFlowAttribute
description: Представляет настраиваемый атрибут потока пользователей в клиентах Azure Active Directory, который можно использовать в потоке пользователей для самостоятельной регистрации.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2bb354ab8028a6d3ca96418c4b0566ea6fe195ef
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883370"
---
# <a name="identitycustomuserflowattribute-resource-type"></a>тип ресурса identityCustomUserFlowAttribute

Пространство имен: microsoft.graph

Представляет настраиваемый атрибут потока пользователей в клиентах Azure Active Directory, который можно использовать в потоке пользователей для самостоятельной регистрации. Эти атрибуты не могут быть изменены и являются только для чтения.

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
