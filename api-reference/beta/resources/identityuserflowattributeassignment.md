---
title: тип ресурса identityUserFlowAttributeAssignment
description: IdentityUserFlowAttributeAssignments используются для сбора определенных identityUserFlowAttributes в потоке пользователей.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a414878e96198443402df7a0c86699e31f8bb690c1157a85ab33118fc8457bc3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54245242"
---
# <a name="identityuserflowattributeassignment-resource-type"></a>тип ресурса identityUserFlowAttributeAssignment

Пространство имен: microsoft.graph

IdentityUserFlowAttributeAssignments используются для сбора определенных identityUserFlowAttributes в потоке пользователей. Это позволяет контролировать атрибуты, собранные в потоке пользователей, и предоставляет параметры настройки для сбора атрибута в потоке пользователей. Вы можете иметь несколько удостоверенийUserFlowAttributeAssignments в одном потоке пользователей, который создает впечатление, которое видит конечный пользователь во время регистрации при запросе предоставить сведения, необходимые потоку пользователей для завершения регистрации.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-get.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Ознакомьтесь с свойствами и отношениями объекта identityUserFlowAttributeAssignment.|
|[Обновление identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-update.md)|Нет|Обновление свойств объекта identityUserFlowAttributeAssignment.|
|[Удаление identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-delete.md)|Нет|Удаление определенного объекта identityUserFlowAttributeAssignment.|
|[getOrder](../api/identityuserflowattributeassignment-getorder.md)|[assignmentOrder](../resources/assignmentorder.md)|Получает порядок сбора identityUserFlowAttributes в потоке пользователей.|
|[setOrder](../api/identityuserflowattributeassignment-setorder.md)|Нет|Задает порядок сбора identityUserFlowAttributes в потоке пользователей.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор identityUserFlowAttributeAssignment. Этот идентификатор неуменяем после создания. Это свойство только для чтения.|
|displayName|Строка|Отображение имени identityUserFlowAttribute в потоке пользователей.|
|isOptional|Логический|Определяет, является ли identityUserFlowAttribute необязательным. `true` означает, что пользователю не нужно предоставлять значение. `false` означает, что пользователь не может завершить регистрацию без предоставления значения.|
|requiresVerification|Логический|Определяет, требуется ли проверка identityUserFlowAttribute. Это используется только для проверки номера телефона или адреса электронной почты пользователя.|
|userAttributeValues|[коллекция userAttributeValuesItem](../resources/userattributevaluesitem.md)|Параметры ввода атрибута потока пользователя. Применимо только в том случае, если userInputType `radioSingleSelect` является `dropdownSingleSelect` , или `checkboxMultiSelect` .|
|userInputType|identityUserFlowAttributeInputType|Тип ввода атрибута потока пользователя. Возможные значения: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|userAttribute|[identityUserFlowAttribute](../resources/identityuserflowattribute.md)|Атрибут пользователя, который необходимо добавить в поток пользователей.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityUserFlowAttributeAssignment",
  "id": "String (identifier)",
  "isOptional": "Boolean",
  "requiresVerification": "Boolean",
  "userInputType": "String",
  "userAttributeValues": [
    {
      "@odata.type": "microsoft.graph.userAttributeValuesItem"
    }
  ],
  "displayName": "String"
}
```
