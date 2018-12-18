---
title: Тип ресурса windowsProtectionState
description: Устройство защиты состояния сущности.
author: tfitzmac
ms.openlocfilehash: 636b969ddafde5976939df764ae1180e19a181c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328079"
---
# <a name="windowsprotectionstate-resource-type"></a>Тип ресурса windowsProtectionState

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Устройство защиты состояния сущности.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение windowsProtectionState](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Чтение свойства и связи объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .|
|[Обновление windowsProtectionState](../api/intune-devices-windowsprotectionstate-update.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Обновление свойства объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для объекта состояния защиты устройств. — Идентификатор устройства, устройства|
|malwareProtectionEnabled|Boolean.|Защита от вредоносных программ включен или не|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|Состояние компьютера (например, очистить или Ожидание полного сканирования или помещенных в очередь перезагрузки и т.). Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|realTimeProtectionEnabled|Boolean.|Защита в режиме реального времени включено или нет?|
|networkInspectionSystemEnabled|Boolean.|Система проверки сети включено или нет?|
|quickScanOverdue|Boolean.|Быстрое сканирование просроченные или не?|
|fullScanOverdue|Boolean.|Полное сканирование просроченные или нет?|
|signatureUpdateOverdue|Boolean.|Устаревший подписи или нет?|
|rebootRequired|Boolean.|Требуется ли перезагрузка?|
|fullScanRequired|Boolean.|Полная проверка, требуется или нет?|
|engineVersion|String.|Версия текущей конечной точки защиты ядра|
|signatureVersion|String.|Текущая версия определения вредоносных программ|
|antiMalwareVersion|String.|Текущая платформа защита от вредоносных программ версии|
|lastQuickScanDateTime|DateTimeOffset|Даты и времени последнего быстрого сканирования|
|lastFullScanDateTime|DateTimeOffset|Даты и времени последнего быстрого сканирования|
|lastQuickScanSignatureVersion|String.|Последняя версия подписи быстрого сканирования|
|lastFullScanSignatureVersion|String.|Последняя версия полная проверка подписи|
|lastReportedDateTime|DateTimeOffset|Последнее состояние работоспособности устройства, обнаруженных времени|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|detectedMalwareState|[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md) коллекции|Список устройств вредоносных программ|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "String (identifier)",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```





