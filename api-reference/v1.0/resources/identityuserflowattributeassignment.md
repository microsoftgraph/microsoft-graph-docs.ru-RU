---
title: тип ресурса identityUserFlowAttributeAssignment
description: Представляет, как атрибуты собираются в потоке пользователей удостоверений.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7be5352030ed56b6d4112ed3409f7969606b5020
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59129903"
---
# <a name="identityuserflowattributeassignment-resource-type"></a>тип ресурса identityUserFlowAttributeAssignment

Пространство имен: microsoft.graph

Представляет, как атрибуты собираются в потоке пользователей удостоверений. Это позволяет настраивать параметры для сбора атрибутов в потоке пользователей. Вы можете иметь несколько удостоверенийUserFlowAttributeAssignments в одном потоке пользователей, что создает возможность предоставления сведений, необходимых пользователю для завершения регистрации.

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

## <a name="relationships"></a>Отношения

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
