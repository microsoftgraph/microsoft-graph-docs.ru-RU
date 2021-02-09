---
title: Тип ресурса identityUserFlowAttributeAssignment
description: identityUserFlowAttributeAssignments используются для сбора определенных identityUserFlowAttributes в пользовательском потоке.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 65859cb0d235454577e236761064f4597f5c68d8
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158788"
---
# <a name="identityuserflowattributeassignment-resource-type"></a>Тип ресурса identityUserFlowAttributeAssignment

Пространство имен: microsoft.graph

identityUserFlowAttributeAssignments используются для сбора определенных identityUserFlowAttributes в пользовательском потоке. Это позволяет управлять атрибутами, собранными в пользовательском потоке, и предоставляет параметры настройки для сбора атрибута в пользовательском потоке. В одном пользовательском потоке может быть несколько удостоверенийUserFlowAttributeAssignment, что создает интерфейс, который видит конечный пользователь во время регистрации при запросе на предоставление сведений, необходимых пользовательскому потоку для завершения регистрации.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-get.md)|[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)|Чтение свойств и связей объекта identityUserFlowAttributeAssignment.|
|[Обновление identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-update.md)|Нет|Обновление свойств объекта identityUserFlowAttributeAssignment.|
|[Удаление identityUserFlowAttributeAssignment](../api/identityuserflowattributeassignment-delete.md)|Нет|Удаление определенного объекта identityUserFlowAttributeAssignment.|
|[getOrder](../api/identityuserflowattributeassignment-getorder.md)|[assignmentOrder](../resources/assignmentorder.md)|Получает порядок identityUserFlowAttributes, собираемого в пользовательском потоке.|
|[setOrder](../api/identityuserflowattributeassignment-setorder.md)|Нет|Задает порядок identityUserFlowAttributes, собираемого в пользовательском потоке.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор identityUserFlowAttributeAssignment. Этот идентификатор не может быть неуявяем после его создания. Это свойство только для чтения.|
|displayName|String|Отображаемого имени identityUserFlowAttribute в пользовательском потоке.|
|isOptional|Boolean|Определяет, является ли identityUserFlowAttribute необязательным. `true` означает, что пользователю не нужно предоставлять значение. `false` означает, что пользователь не может завершить регистрацию без предоставления значения.|
|requiresVerification|Boolean|Определяет, требуется ли проверка identityUserFlowAttribute. Он используется только для проверки номера телефона или адреса электронной почты пользователя.|
|userAttributeValues|[Коллекция userAttributeValuesItem](../resources/userattributevaluesitem.md)|Параметры ввода для атрибута пользовательского потока. Применимо только в том случае, если userInputType имеет , `radioSingleSelect` `dropdownSingleSelect` или `checkboxMultiSelect` .|
|userInputType|identityUserFlowAttributeInputType|Тип ввода атрибута пользовательского потока. Возможные значения: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|userAttribute|[identityUserFlowAttribute](../resources/identityuserflowattribute.md)|Атрибут пользователя, который вы хотите добавить в пользовательский поток.|

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
