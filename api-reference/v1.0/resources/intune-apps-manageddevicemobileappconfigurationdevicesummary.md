---
title: Тип ресурса managedDeviceMobileAppConfigurationDeviceSummary
description: Содержит свойства, унаследованные свойства и действия из сводки по состоянию конфигурации мобильных приложений MDM для устройства.
ms.openlocfilehash: 459d97fd57987fba1c760f1c716553fa71233c2f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028196"
---
# <a name="manageddevicemobileappconfigurationdevicesummary-resource-type"></a>Тип ресурса managedDeviceMobileAppConfigurationDeviceSummary

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства, унаследованные свойства и действия из сводки по состоянию конфигурации мобильных приложений MDM для устройства.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта managedDeviceMobileAppConfigurationDeviceSummary](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-get.md)|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|Чтение свойств и связей объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).|
|[Обновление объекта managedDeviceMobileAppConfigurationDeviceSummary](../api/intune-apps-manageddevicemobileappconfigurationdevicesummary-update.md)|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|Обновление свойств объекта [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|pendingCount|Int32|Количество ожидающих устройств.|
|notApplicableCount|Int32|Количество неприменимых устройств.|
|successCount|Int32|Количество успешных устройств.|
|errorCount|Int32|Количество устройств с ошибками.|
|failedCount|Int32|Число устройств со сбоями.|
|lastUpdateDateTime|DateTimeOffset|Время последнего обновления.|
|configurationVersion|Int32|Версия политики для этого обзора|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```



