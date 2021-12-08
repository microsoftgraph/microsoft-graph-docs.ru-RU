---
title: тип ресурса hardwareConfigurationRunSummary
description: Содержит свойства для сводки запуска сценария конфигурации оборудования.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6debf44d50ff1f501af172de706165c22dd02642
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345621"
---
# <a name="hardwareconfigurationrunsummary-resource-type"></a>тип ресурса hardwareConfigurationRunSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для сводки запуска сценария конфигурации оборудования.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get hardwareConfigurationRunSummary](../api/intune-deviceconfig-hardwareconfigurationrunsummary-get.md)|[hardwareConfigurationRunSummary](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)|Чтение свойств и связей объекта [hardwareConfigurationRunSummary.](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)|
|[Обновление hardwareConfigurationRunSummary](../api/intune-deviceconfig-hardwareconfigurationrunsummary-update.md)|[hardwareConfigurationRunSummary](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)|Обновление свойств объекта [hardwareConfigurationRunSummary.](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Клавиша конфигурации оборудования выполнить сводную сущность. Это свойство доступно только для чтения.|
|successfulDeviceCount|Int32|Количество устройств, для которых оборудование настроено без проблем|
|failedDeviceCount|Int32|Количество устройств, для которых конфигурация оборудования обнаружила проблему|
|pendingDeviceCount|Int32|Количество устройств, для которых конфигурация оборудования находится в ожидаемом состоянии|
|errorDeviceCount|Int32|Количество устройств, для которых состояние конфигурации оборудования является ошибкой|
|notApplicableDeviceCount|Int32|Количество устройств, для которых не применимо состояние конфигурации оборудования|
|unknownDeviceCount|Int32|Количество устройств, для которых неизвестно состояние конфигурации оборудования|
|successfulUserCount|Int32|Число пользователей, для которых оборудование настроено без каких-либо проблем|
|failedUserCount|Int32|Число пользователей, для которых конфигурация оборудования обнаружила проблему|
|pendingUserCount|Int32|Число пользователей, для которых конфигурация оборудования находится в ожидаемом состоянии|
|errorUserCount|Int32|Число пользователей, для которых состояние конфигурации оборудования является ошибкой|
|notApplicableUserCount|Int32|Число пользователей, для которых не применимо состояние конфигурации оборудования|
|unknownUserCount|Int32|Число пользователей, для которых неизвестно состояние конфигурации оборудования|
|lastRunDateTime|DateTimeOffset|Время последнего запуска конфигурации на всех устройствах|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwareConfigurationRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareConfigurationRunSummary",
  "id": "String (identifier)",
  "successfulDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "pendingDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "successfulUserCount": 1024,
  "failedUserCount": 1024,
  "pendingUserCount": 1024,
  "errorUserCount": 1024,
  "notApplicableUserCount": 1024,
  "unknownUserCount": 1024,
  "lastRunDateTime": "String (timestamp)"
}
```




