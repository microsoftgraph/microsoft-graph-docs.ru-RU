---
title: тип ресурса windowsProtectionState
description: Объект состояния защиты устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 640198171fd9b83c6522a8c8b07b84fa186657ab
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803239"
---
# <a name="windowsprotectionstate-resource-type"></a>тип ресурса windowsProtectionState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект состояния защиты устройств.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get windowsProtectionState](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Чтение свойств и связей [объекта WindowsProtectionState.](../resources/intune-devices-windowsprotectionstate.md)|
|[Обновление windowsProtectionState](../api/intune-devices-windowsprotectionstate-update.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Обновление свойств объекта [WindowsProtectionState.](../resources/intune-devices-windowsprotectionstate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для объекта защиты от устройства. Это id устройства|
|malwareProtectionEnabled|Логический|Включено или не включено вредоносное ПО|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|Состояние компьютера (например, очистка или ожидание полного сканирования или ожидающих перезагрузки и т.д.). Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|realTimeProtectionEnabled|Boolean|Включена защита в режиме реального времени или нет?|
|networkInspectionSystemEnabled|Логический|Включена или нет включена система сетевого контроля?|
|quickScanOverdue|Логический|Быстрое сканирование просрочено или нет?|
|fullScanOverdue|Логический|Полная просроченная проверка или нет?|
|signatureUpdateOverdue|Boolean|Подпись устарела или нет?|
|rebootRequired|Логический|Перезагрузка требуется или нет?|
|fullScanRequired|Boolean|Полное сканирование требуется или нет?|
|engineVersion|Строка|Версия двигателя защиты конечной точки|
|signatureVersion|Строка|Текущая версия определений вредоносных программ|
|antiMalwareVersion|Строка|Текущая версия антивирусных программ|
|lastQuickScanDateTime|DateTimeOffset|Дата последнего быстрого сканирования|
|lastFullScanDateTime|DateTimeOffset|Дата последнего быстрого сканирования|
|lastQuickScanSignatureVersion|Строка|Последняя версия подписи быстрого сканирования|
|lastFullScanSignatureVersion|Строка|Последняя версия подписи полного сканирования|
|lastReportedDateTime|DateTimeOffset|Время последнего состояния состояния устройства|
|productStatus|[windowsDefenderProductStatus](../resources/intune-devices-windowsdefenderproductstatus.md)|Состояние продукта антивирусная программа . Возможные значения: `noStatus` `serviceNotRunning` , `serviceStartedWithoutMalwareProtection` `pendingFullScanDueToThreatAction` `pendingRebootDueToThreatAction` `pendingManualStepsDueToThreatAction` `avSignaturesOutOfDate` `asSignaturesOutOfDate` `noQuickScanHappenedForSpecifiedPeriod` `noFullScanHappenedForSpecifiedPeriod` `systemInitiatedScanInProgress` `systemInitiatedCleanInProgress` `samplesPendingSubmission` `productRunningInEvaluationMode` `productRunningInNonGenuineMode` `productExpired` `offlineScanRequired` `serviceShutdownAsPartOfSystemShutdown` `threatRemediationFailedCritically` `threatRemediationFailedNonCritically` `noStatusFlagsSet` `platformOutOfDate` `platformUpdateInProgress` `platformAboutToBeOutdated` `signatureOrPlatformEndOfLifeIsPastOrIsImpending` . `windowsSModeSignaturesInUseOnNonWin10SInstall`|
|isVirtualMachine|Boolean|Указывает, является ли устройство виртуальной машиной.|
|tamperProtectionEnabled|Логический|Указывает, включена ли Защитник Windows защита от взлома.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|detectedMalwareState|[коллекция windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)|Список вредоносных программ устройств|

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
  "lastReportedDateTime": "String (timestamp)",
  "productStatus": "String",
  "isVirtualMachine": true,
  "tamperProtectionEnabled": true
}
```



