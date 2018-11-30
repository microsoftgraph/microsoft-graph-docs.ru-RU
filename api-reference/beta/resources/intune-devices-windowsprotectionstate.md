---
title: Тип ресурса windowsProtectionState
description: Устройство защиты состояния сущности.
ms.openlocfilehash: dfdfb5f79f696e2f6f577f59b7597f16c89a5d56
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081581"
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
|id|String|Уникальный идентификатор для объекта состояния защиты устройств. — Идентификатор устройства, устройства|
|malwareProtectionEnabled|Логический|Защита от вредоносных программ включен или не|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|Состояние компьютера (например, очистить или Ожидание полного сканирования или помещенных в очередь перезагрузки и т.). Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|realTimeProtectionEnabled|Логический|Защита в режиме реального времени включено или нет?|
|networkInspectionSystemEnabled|Логический|Система проверки сети включено или нет?|
|quickScanOverdue|Логический|Быстрое сканирование просроченные или не?|
|fullScanOverdue|Логический|Полное сканирование просроченные или нет?|
|signatureUpdateOverdue|Логический|Устаревший подписи или нет?|
|rebootRequired|Логический|Требуется ли перезагрузка?|
|fullScanRequired|Логический|Полная проверка, требуется или нет?|
|engineVersion|String|Версия текущей конечной точки защиты ядра|
|signatureVersion|String|Текущая версия определения вредоносных программ|
|antiMalwareVersion|String|Текущая платформа защита от вредоносных программ версии|
|lastQuickScanDateTime|DateTimeOffset|Даты и времени последнего быстрого сканирования|
|lastFullScanDateTime|DateTimeOffset|Даты и времени последнего быстрого сканирования|
|lastQuickScanSignatureVersion|String|Последняя версия подписи быстрого сканирования|
|lastFullScanSignatureVersion|String|Последняя версия полная проверка подписи|
|lastReportedDateTime|DateTimeOffset|Последнее состояние работоспособности устройства, обнаруженных времени|

## <a name="relationships"></a>Связи
|Связь|Тип|Description|
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





