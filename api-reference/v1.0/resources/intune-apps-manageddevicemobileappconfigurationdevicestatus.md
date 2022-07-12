---
title: Тип ресурса managedDeviceMobileAppConfigurationDeviceStatus
description: Содержит свойства, унаследованные свойства и действия для состояния конфигурации мобильного приложения MDM для устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 97544b5f98165f09e4cdfbb69d59759e6d850282
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66733915"
---
# <a name="manageddevicemobileappconfigurationdevicestatus-resource-type"></a>Тип ресурса managedDeviceMobileAppConfigurationDeviceStatus

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, унаследованные свойства и действия для состояния конфигурации мобильного приложения MDM для устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов managedDeviceMobileAppConfigurationDeviceStatuses](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-list.md)|[Коллекция managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|Список свойств и связей объектов [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .|
|[Получение managedDeviceMobileAppConfigurationDeviceStatus](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-get.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .|
|[Создание объекта managedDeviceMobileAppConfigurationDeviceStatus](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-create.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|Создайте объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .|
|[Удаление объекта managedDeviceMobileAppConfigurationDeviceStatus](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-delete.md)|Нет|Удаляет [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).|
|[Обновление объекта managedDeviceMobileAppConfigurationDeviceStatus](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-update.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|deviceDisplayName|String|Имя устройства в объекте DevicePolicyStatus.|
|userName|String|Имя пользователя в отчете|
|deviceModel|String|Модель устройства в отчете|
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
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
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





