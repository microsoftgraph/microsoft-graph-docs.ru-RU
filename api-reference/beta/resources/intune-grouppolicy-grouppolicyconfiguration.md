---
title: Тип ресурса Граупполициконфигуратион
description: Объект конфигурации групповой политики содержит настроенные значения для одного или нескольких определений групповой политики.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 540da94d92f3056a6699b7112f3589f6da4b7144
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160755"
---
# <a name="grouppolicyconfiguration-resource-type"></a>Тип ресурса Граупполициконфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект конфигурации групповой политики содержит настроенные значения для одного или нескольких определений групповой политики.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполициконфигуратионс](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|Коллекция [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Список свойств и связей объектов [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .|
|[Получение Граупполициконфигуратион](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[Граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Чтение свойств и связей объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .|
|[Создание Граупполициконфигуратион](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[Граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Создание нового объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .|
|[Удаление Граупполициконфигуратион](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|Нет|Удаляет объект [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md).|
|[Обновление Граупполициконфигуратион](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[Граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Обновление свойств объекта [граупполициконфигуратион](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .|
|[Действие assign](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|Коллекция [граупполициконфигуратионассигнмент](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|displayName|String|Предоставленное пользователем имя объекта ресурса.|
|description|String|Предоставленное пользователем описание объекта ресурса.|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|Дефинитионвалуес|Коллекция [граупполицидефинитионвалуе](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Список включенных или отключенных значений определений групповой политики для конфигурации.|
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
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




