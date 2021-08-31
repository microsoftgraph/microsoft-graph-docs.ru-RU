---
title: Тип ресурса settingStateDeviceSummary
description: Сводка по состоянию параметра конфигурации и политики соответствия требованиям для устройств
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 562c63e93e0003bff08351878ca07c64b3eefd49
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796238"
---
# <a name="settingstatedevicesummary-resource-type"></a>Тип ресурса settingStateDeviceSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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



