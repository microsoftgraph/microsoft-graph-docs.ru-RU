---
title: Тип ресурса Граупполициконфигуратион
description: Объект конфигурации групповой политики содержит настроенные значения для одного или нескольких определений групповой политики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e4fce57585c0dee4f73719870da7d07a2d710cd5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267196"
---
# <a name="grouppolicyconfiguration-resource-type"></a>Тип ресурса Граупполициконфигуратион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект конфигурации групповой политики содержит настроенные значения для одного или нескольких определений групповой политики.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполициконфигуратионс](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|Коллекция [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Список свойств и связей объектов [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .|
|[Получение Граупполициконфигуратион](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Чтение свойств и связей объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .|
|[Создание Граупполициконфигуратион](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Создание нового объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .|
|[Удаление Граупполициконфигуратион](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|Нет|Удаляет объект [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md).|
|[Обновление Граупполициконфигуратион](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Обновление свойств объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .|
|[Действие assign](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Пока не задокументировано.|
|[действие Упдатедефинитионвалуес](../api/intune-grouppolicy-grouppolicyconfiguration-updatedefinitionvalues.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|displayName|String|Предоставленное пользователем имя объекта ресурса.|
|description|String|Предоставленное пользователем описание объекта ресурса.|
|roleScopeTagIds|Коллекция строк|Список тегов области для конфигурации.|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|дефинитионвалуес|Коллекция [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Список включенных или отключенных значений определений групповой политики для конфигурации.|
|assignments|Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Список назначений групп для конфигурации.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




