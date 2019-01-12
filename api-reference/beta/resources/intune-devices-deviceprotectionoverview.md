---
title: Тип ресурса deviceProtectionOverview
description: Сведения об оборудовании данного устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f7b7c28474692c1b1df3b1d6a703e3dd43d05a15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944322"
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





