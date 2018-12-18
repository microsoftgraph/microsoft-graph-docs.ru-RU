---
title: Тип ресурса deviceProtectionOverview
description: Сведения об оборудовании данного устройства.
author: tfitzmac
ms.openlocfilehash: e705324bfc611117657ec629f8770e76c69be28d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317054"
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





