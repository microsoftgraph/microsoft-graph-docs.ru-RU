---
title: Тип ресурса Девицеконфигуратионконфликтсуммари
description: Сводка по конфликтам для набора политик конфигурации устройств.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3ce50b49c34427f1cde7011fb76e566a1e45ba9f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333018"
---
# <a name="deviceconfigurationconflictsummary-resource-type"></a>Тип ресурса Девицеконфигуратионконфликтсуммари

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка по конфликтам для набора политик конфигурации устройств.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеконфигуратионконфликтсуммариес](../api/intune-deviceconfig-deviceconfigurationconflictsummary-list.md)|Коллекция [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Список свойств и связей объектов [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .|
|[Получение Девицеконфигуратионконфликтсуммари](../api/intune-deviceconfig-deviceconfigurationconflictsummary-get.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Чтение свойств и связей объекта [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .|
|[Создание Девицеконфигуратионконфликтсуммари](../api/intune-deviceconfig-deviceconfigurationconflictsummary-create.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Создание нового объекта [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .|
|[Удаление Девицеконфигуратионконфликтсуммари](../api/intune-deviceconfig-deviceconfigurationconflictsummary-delete.md)|Нет|Удаляет объект [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).|
|[Обновление Девицеконфигуратионконфликтсуммари](../api/intune-deviceconfig-deviceconfigurationconflictsummary-update.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Обновление свойств объекта [девицеконфигуратионконфликтсуммари](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|конфликтингдевицеконфигуратионс|Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)|Набор политик в конфликте с заданным параметром|
|id|String|Идентификатор этого набора конфликтующих политик. Этот идентификатор — идентификаторы всех политик в Конфликтингдевицеконфигуратионс в лексикографикал порядке, разделенных символами подчеркивания.|
|контрибутингсеттингс|Коллекция строк|Набор параметров в конфликте с заданными политиками|
|девицечеккинсимпактед|Int32|Число возвратов, затронутых конфликтующими политиками и параметрами|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationConflictSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "id": "String (identifier)",
  "contributingSettings": [
    "String"
  ],
  "deviceCheckinsImpacted": 1024
}
```



