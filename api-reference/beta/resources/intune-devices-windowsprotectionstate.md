---
title: Тип ресурса windowsProtectionState
description: Устройство защиты состояния сущности.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5a21cc27039f3119836e0027b2558cadadab1b5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884107"
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
|malwareProtectionEnabled|Логический|Защита от вредоносных программ включен или не|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|Состояние компьютера (например, очистить или Ожидание полного сканирования или помещенных в очередь перезагрузки и т.). Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|realTimeProtectionEnabled|Логический|Защита в режиме реального времени включено или нет?|
|networkInspectionSystemEnabled|Логический|Система проверки сети включено или нет?|
|quickScanOverdue|Логический|Быстрое сканирование просроченные или не?|
|fullScanOverdue|Логический|Полное сканирование просроченные или нет?|
|signatureUpdateOverdue|Логический|Устаревший подписи или нет?|
|rebootRequired|Логический|Требуется ли перезагрузка?|
|fullScanRequired|Логический|Полная проверка, требуется или нет?|
|engineVersion|Строка|Версия текущей конечной точки защиты ядра|
|signatureVersion|Строка|Текущая версия определения вредоносных программ|
|antiMalwareVersion|Строка|Текущая платформа защита от вредоносных программ версии|
|lastQuickScanDateTime|DateTimeOffset|Даты и времени последнего быстрого сканирования|
|lastFullScanDateTime|DateTimeOffset|Даты и времени последнего быстрого сканирования|
|lastQuickScanSignatureVersion|Строка|Последняя версия подписи быстрого сканирования|
|lastFullScanSignatureVersion|Строка|Последняя версия полная проверка подписи|
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





