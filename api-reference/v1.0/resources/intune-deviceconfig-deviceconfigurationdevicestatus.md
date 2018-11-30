---
title: Тип ресурса deviceConfigurationDeviceStatus
description: Н/Д
ms.openlocfilehash: c3e4df1b83c92ea5817bdfd8013015eb4dd29ce2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025114"
---
# <a name="deviceconfigurationdevicestatus-resource-type"></a>Тип ресурса deviceConfigurationDeviceStatus

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Н/Д
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceConfigurationDeviceStatus](../api/intune-deviceconfig-deviceconfigurationdevicestatus-list.md)|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Список свойств и связей объектов [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).|
|[Получение объекта deviceConfigurationDeviceStatus](../api/intune-deviceconfig-deviceconfigurationdevicestatus-get.md)|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Чтение свойств и связей объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).|
|[Создание объекта deviceConfigurationDeviceStatus](../api/intune-deviceconfig-deviceconfigurationdevicestatus-create.md)|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Создание объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).|
|[Удаление объекта deviceConfigurationDeviceStatus](../api/intune-deviceconfig-deviceconfigurationdevicestatus-delete.md)|Нет|Удаляет объект [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).|
|[Обновление объекта deviceConfigurationDeviceStatus](../api/intune-deviceconfig-deviceconfigurationdevicestatus-update.md)|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Обновление свойств объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|deviceDisplayName|String|Имя устройства в объекте DevicePolicyStatus.|
|userName|String|Имя пользователя в отчете.|
|deviceModel|String|Модель устройства в отчете.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|Дата и время, когда истекает период отсрочки применения политик на устройстве.|
|status|[complianceStatus](../resources/intune-shared-compliancestatus.md)|Состояние соответствия требованиям для отчета о политике. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|lastReportedDateTime|DateTimeOffset|Дата и время последнего изменения отчета о политике.|
|userPrincipalName|String|Имя участника-пользователя.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



