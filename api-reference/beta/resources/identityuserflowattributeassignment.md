---
title: Тип ресурса Идентитюсерфловаттрибутеассигнмент
description: Идентитюсерфловаттрибутеассигнментс используются для сбора определенных Идентитюсерфловаттрибутес в рамках пользовательского процесса.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 80bc6547307914e0d206ea9b5c79073f96fce19c
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581345"
---
# <a name="identityuserflowattributeassignment-resource-type"></a>Тип ресурса Идентитюсерфловаттрибутеассигнмент

Пространство имен: microsoft.graph

Идентитюсерфловаттрибутеассигнментс используются для сбора определенных Идентитюсерфловаттрибутес в рамках пользовательского процесса. Это позволяет управлять атрибутами, собранными в пользовательском цикле, и предоставляет варианты настройки для сбора атрибута в пределах пользовательского процесса. Вы можете использовать несколько Идентитюсерфловаттрибутеассигнментс в одном потоке пользователей, который создает интерфейс, который видит конечный пользователь во время регистрации, когда вам будет предложено предоставить сведения, необходимые для входа пользователя в систему.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение Идентитюсерфловаттрибутеассигнмент](../api/identityuserflowattributeassignment-get.md)|[идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md)|Чтение свойств и связей объекта Идентитюсерфловаттрибутеассигнмент.|
|[Обновление Идентитюсерфловаттрибутеассигнмент](../api/identityuserflowattributeassignment-update.md)|Нет|Обновление свойств объекта Идентитюсерфловаттрибутеассигнмент.|
|[Удаление Идентитюсерфловаттрибутеассигнмент](../api/identityuserflowattributeassignment-delete.md)|Нет|Удаление определенного объекта Идентитюсерфловаттрибутеассигнмент.|
|[по убыванию](../api/identityuserflowattributeassignment-getorder.md)|[ассигнментордер](../resources/assignmentorder.md)|Получает порядок Идентитюсерфловаттрибутес, собранных в пользовательском движении.|
|[сетордер](../api/identityuserflowattributeassignment-setorder.md)|Нет|Задает порядок Идентитюсерфловаттрибутес, собранных в пользовательском движении.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор Идентитюсерфловаттрибутеассигнмент. Этот идентификатор становится неизменяемым после его создания. Это свойство доступно только для чтения.|
|displayName|String|Отображаемое имя Идентитюсерфловаттрибуте в пользовательском движении.|
|Переключатель|Логический|Определяет, является ли Идентитюсерфловаттрибуте необязательным. `true` означает, что пользователю не нужно указывать значение. `false` означает, что пользователь не может выполнить вход, не указывая значение.|
|рекуиресверификатион|Логический|Определяет, требуется ли для Идентитюсерфловаттрибуте проверка. Используется только для проверки номера телефона пользователя или адреса электронной почты.|
|усераттрибутевалуес|Коллекция [усераттрибутевалуеситем](../resources/userattributevaluesitem.md)|Параметры ввода для атрибута Flow User. Применяется только в том случае, если для Усеринпуттипе задано значение `radioSingleSelect` , `dropdownSingleSelect` или `checkboxMultiSelect` .|
|усеринпуттипе|идентитюсерфловаттрибутеинпуттипе|Тип входных данных для атрибута Flow User. Возможные значения: `textBox`, `dateTimeDropdown`, `radioSingleSelect`, `dropdownSingleSelect`, `emailBox`, `checkboxMultiSelect`.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|усераттрибуте|[идентитюсерфловаттрибуте](../resources/identityuserflowattribute.md)|Атрибут пользователя, который требуется добавить в пользовательский блок.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment",
  "baseType": "",
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
