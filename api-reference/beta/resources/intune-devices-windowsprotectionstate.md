---
title: тип ресурса windowsProtectionState
description: Объект состояния защиты устройств.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 39ee7f404ffc54a31a29fec2cac5f6876884f1db
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59040010"
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
|id|String|Уникальный идентификатор для объекта защиты от устройства. Это id устройства|
|malwareProtectionEnabled|Логический|Включено или не включено вредоносное ПО|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|Состояние компьютера (например, очистка или ожидание полного сканирования или ожидающих перезагрузки и т.д.). Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|realTimeProtectionEnabled|Логическое|Включена защита в режиме реального времени или нет?|
|networkInspectionSystemEnabled|Логическое|Включена или нет включена система сетевого контроля?|
|quickScanOverdue|Логический|Быстрое сканирование просрочено или нет?|
|fullScanOverdue|Логический|Полная просроченная проверка или нет?|
|signatureUpdateOverdue|Логическое|Подпись устарела или нет?|
|rebootRequired|Логическое|Перезагрузка требуется или нет?|
|fullScanRequired|Логический|Полное сканирование требуется или нет?|
|engineVersion|String|Версия двигателя защиты конечной точки|
|signatureVersion|String|Текущая версия определений вредоносных программ|
|antiMalwareVersion|String|Текущая версия антивирусных программ|
|lastQuickScanDateTime|DateTimeOffset|Дата последнего быстрого сканирования|
|lastFullScanDateTime|DateTimeOffset|Дата последнего быстрого сканирования|
|lastQuickScanSignatureVersion|String|Последняя версия подписи быстрого сканирования|
|lastFullScanSignatureVersion|String|Последняя версия подписи полного сканирования|
|lastReportedDateTime|DateTimeOffset|Время последнего состояния состояния устройства|
|productStatus|[windowsDefenderProductStatus](../resources/intune-devices-windowsdefenderproductstatus.md)|Состояние продукта антивирусная программа . Возможные значения: `noStatus` `serviceNotRunning` , `serviceStartedWithoutMalwareProtection` `pendingFullScanDueToThreatAction` `pendingRebootDueToThreatAction` `pendingManualStepsDueToThreatAction` `avSignaturesOutOfDate` `asSignaturesOutOfDate` `noQuickScanHappenedForSpecifiedPeriod` `noFullScanHappenedForSpecifiedPeriod` `systemInitiatedScanInProgress` `systemInitiatedCleanInProgress` `samplesPendingSubmission` `productRunningInEvaluationMode` `productRunningInNonGenuineMode` `productExpired` `offlineScanRequired` `serviceShutdownAsPartOfSystemShutdown` `threatRemediationFailedCritically` `threatRemediationFailedNonCritically` `noStatusFlagsSet` `platformOutOfDate` `platformUpdateInProgress` `platformAboutToBeOutdated` `signatureOrPlatformEndOfLifeIsPastOrIsImpending` . `windowsSModeSignaturesInUseOnNonWin10SInstall`|
|isVirtualMachine|Логический|Указывает, является ли устройство виртуальной машиной.|
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



