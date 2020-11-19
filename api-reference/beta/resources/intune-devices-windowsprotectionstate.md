---
title: Тип ресурса windowsProtectionState
description: Объект состояния защиты устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b2651aa9fad173654d8fff554bdf89f7ab36da14
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49207563"
---
# <a name="windowsprotectionstate-resource-type"></a>Тип ресурса windowsProtectionState

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект состояния защиты устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение windowsProtectionState](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Чтение свойств и связей объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .|
|[Обновление windowsProtectionState](../api/intune-devices-windowsprotectionstate-update.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для объекта состояния защиты устройства. Это идентификатор устройства для устройства.|
|малварепротектионенаблед|Boolean|Защита от вредоносных программ включена или нет|
|девицестате|[виндовсдевицехеалсстате](../resources/intune-devices-windowsdevicehealthstate.md)|Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.). Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|реалтимепротектионенаблед|Boolean|Защита в режиме реального времени включена или нет?|
|нетворкинспектионсистеменаблед|Boolean|Система проверки сети включена или нет?|
|куиккскановердуе|Boolean|Быстрая проверка просрочена или нет?|
|фуллскановердуе|Boolean|Полная проверка просрочена или нет?|
|сигнатуреупдатеовердуе|Boolean|Подпись устарела или нет?|
|ребутрекуиред|Boolean|Требуется перезагрузка или нет?|
|фуллсканрекуиред|Boolean|Необходима полная проверка или нет?|
|енгиневерсион|String|Текущая версия модуля Endpoint Protection|
|сигнатуреверсион|String|Текущая версия определений вредоносных программ|
|антималвареверсион|String|Текущая версия защиты от вредоносных программ|
|ласткуиккскандатетиме|DateTimeOffset|Дата и время последнего быстрого сканирования|
|ластфуллскандатетиме|DateTimeOffset|Дата и время последнего быстрого сканирования|
|ласткуиккскансигнатуреверсион|String|Последняя версия подписи быстрого сканирования|
|ластфуллскансигнатуреверсион|String|Версия последней полной проверки подписи|
|lastReportedDateTime|DateTimeOffset|Последнее состояние работоспособности устройства в отчете о времени|
|продуктстатус|[виндовсдефендерпродуктстатус](../resources/intune-devices-windowsdefenderproductstatus.md)|Состояние продукта антивирусной программы "Защитник Windows". Возможные значения:,,,,,,,,,,, `noStatus` `serviceNotRunning` `serviceStartedWithoutMalwareProtection` `pendingFullScanDueToThreatAction` `pendingRebootDueToThreatAction` `pendingManualStepsDueToThreatAction` `avSignaturesOutOfDate` `asSignaturesOutOfDate` `noQuickScanHappenedForSpecifiedPeriod` `noFullScanHappenedForSpecifiedPeriod` `systemInitiatedScanInProgress` ,,,,,,, `systemInitiatedCleanInProgress` `samplesPendingSubmission` , `productRunningInEvaluationMode` , `productRunningInNonGenuineMode` , `productExpired` `offlineScanRequired` `serviceShutdownAsPartOfSystemShutdown` `threatRemediationFailedCritically` `threatRemediationFailedNonCritically` `noStatusFlagsSet` `platformOutOfDate` `platformUpdateInProgress` `platformAboutToBeOutdated` `signatureOrPlatformEndOfLifeIsPastOrIsImpending` `windowsSModeSignaturesInUseOnNonWin10SInstall` ,,,,,,,,,,,,,,,,,.|
|исвиртуалмачине|Boolean|Указывает, является ли устройство виртуальной машиной.|
|тамперпротектионенаблед|Boolean|Указывает, включена ли функция защиты от несанкционированного защитника Windows.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|детектедмалварестате|Коллекция [виндовсдевицемалварестате](../resources/intune-devices-windowsdevicemalwarestate.md)|Список вредоносных программ для устройств|

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




