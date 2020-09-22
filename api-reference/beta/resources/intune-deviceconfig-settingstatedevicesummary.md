---
title: Тип ресурса settingStateDeviceSummary
description: Сводка по состоянию параметра конфигурации и политики соответствия требованиям для устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed705b12c35c4414913ca0bd3686191f00941449
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049417"
---
# <a name="settingstatedevicesummary-resource-type"></a>Тип ресурса settingStateDeviceSummary

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка по состоянию параметра конфигурации и политики соответствия требованиям для устройств

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов settingStateDeviceSummary](../api/intune-deviceconfig-settingstatedevicesummary-list.md)|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Список свойств и связей объектов [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).|
|[Получение объекта settingStateDeviceSummary](../api/intune-deviceconfig-settingstatedevicesummary-get.md)|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Чтение свойств и связей объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).|
|[Создание объекта settingStateDeviceSummary](../api/intune-deviceconfig-settingstatedevicesummary-create.md)|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Создание объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).|
|[Удаление объекта settingStateDeviceSummary](../api/intune-deviceconfig-settingstatedevicesummary-delete.md)|Нет|Удаляет объект [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).|
|[Обновление объекта settingStateDeviceSummary](../api/intune-deviceconfig-settingstatedevicesummary-update.md)|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Обновление свойств объекта [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|settingName|String|Имя параметра.|
|instancePath|String|Имя пути к экземпляру для параметра.|
|unknownDeviceCount|Int32|Количество неизвестных устройств для параметра.|
|notApplicableDeviceCount|Int32|Количество неприменимых устройств для параметра.|
|compliantDeviceCount|Int32|Количество соответствующих устройств для параметра.|
|remediatedDeviceCount|Int32|Количество соответствующих устройств для параметра.|
|nonCompliantDeviceCount|Int32|Количество несоответствующих устройств для параметра.|
|errorDeviceCount|Int32|Количество ошибок устройств для параметра.|
|conflictDeviceCount|Int32|Количество конфликтов устройств для параметра|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.settingStateDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "instancePath": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```






