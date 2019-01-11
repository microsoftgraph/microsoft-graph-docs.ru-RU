---
title: Тип ресурса deviceProtectionOverview
description: Сведения об оборудовании данного устройства.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 12066877e380c022a1cd1ec49322ab51b8e59d65
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811531"
---
# <a name="deviceprotectionoverview-resource-type"></a>Тип ресурса deviceProtectionOverview

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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

## <a name="relationships"></a>Связи
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





