---
title: Тип ресурса deviceConfigurationConflictSummary
description: Конфликт сводки для набора политик конфигурации устройства.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f8d84a4240059ff9772fefd9737ad27d8fbae7a8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843339"
---
# <a name="deviceconfigurationconflictsummary-resource-type"></a>Тип ресурса deviceConfigurationConflictSummary

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Конфликт сводки для набора политик конфигурации устройства.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceConfigurationConflictSummaries](../api/intune-deviceconfig-deviceconfigurationconflictsummary-list.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) коллекции|Свойства списка и связей объектов [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .|
|[Получение deviceConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-get.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Чтение свойства и связи объекта [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .|
|[Создание deviceConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-create.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Создание нового объекта [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .|
|[Удаление deviceConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-delete.md)|Нет|Удаляет [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).|
|[Обновление deviceConfigurationConflictSummary](../api/intune-deviceconfig-deviceconfigurationconflictsummary-update.md)|[deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)|Обновление свойства объекта [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|conflictingDeviceConfigurations|Коллекция [settingSource](../resources/intune-deviceconfig-settingsource.md)|Набор политик конфликтует с данного параметра|
|id|Строка|Идентификатор для этого набора конфликтующие политики. Этот идентификатор — идентификаторы всех политик в ConflictingDeviceConfigurations в лексикографических порядке, разделенных точкой с подчеркивания.|
|contributingSettings|Коллекция String|Набор параметров конфликтует с указанной политики|
|deviceCheckinsImpacted|Int32|Count возвраты, на которые оказывает влияние конфликтующие политики и параметры|

## <a name="relationships"></a>Связи
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





