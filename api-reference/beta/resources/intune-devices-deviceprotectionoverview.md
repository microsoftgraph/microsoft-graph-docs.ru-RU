---
title: Тип ресурса deviceProtectionOverview
description: Сведения об оборудовании данного устройства.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 902e3a6062d2aa50c96c27eb9d542905bf9a029d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418990"
---
# <a name="deviceprotectionoverview-resource-type"></a>Тип ресурса deviceProtectionOverview

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сведения об оборудовании данного устройства.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|totalReportedDeviceCount|Int32|Счетчик общее устройства.|
|inactiveThreatAgentDeviceCount|Int32|Устройства со счетчиком агента неактивных угроз|
|unknownStateThreatAgentDeviceCount|Int32|Устройство с состоянием агента угроз, как число неизвестно.|
|pendingSignatureUpdateDeviceCount|Int32|Устройство со старой счетчиком подписи.|
|cleanDeviceCount|Int32|Счетчик чистой устройства.|
|pendingFullScanDeviceCount|Int32|Счетчик устройства ожидающие полную проверку.|
|pendingRestartDeviceCount|Int32|Счетчик отложенная перезагрузка устройства.|
|pendingManualStepsDeviceCount|Int32|Счетчик устройства ожидающие ручные операции.|
|pendingOfflineScanDeviceCount|Int32|Число ожидающих автономной проверки устройства.|
|criticalFailuresDeviceCount|Int32|Счетчик устройства критические ошибки.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceProtectionOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceProtectionOverview",
  "totalReportedDeviceCount": 1024,
  "inactiveThreatAgentDeviceCount": 1024,
  "unknownStateThreatAgentDeviceCount": 1024,
  "pendingSignatureUpdateDeviceCount": 1024,
  "cleanDeviceCount": 1024,
  "pendingFullScanDeviceCount": 1024,
  "pendingRestartDeviceCount": 1024,
  "pendingManualStepsDeviceCount": 1024,
  "pendingOfflineScanDeviceCount": 1024,
  "criticalFailuresDeviceCount": 1024
}
```




