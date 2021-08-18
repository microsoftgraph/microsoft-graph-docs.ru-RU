---
title: Обновление windowsProtectionState
description: Обновление свойств объекта WindowsProtectionState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9a8c51bc95de38ddfebc394b50cfdf3dcd12fe74
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58263865"
---
# <a name="update-windowsprotectionstate"></a>Обновление windowsProtectionState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [WindowsProtectionState.](../resources/intune-devices-windowsprotectionstate.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса подарйте представление JSON для [объекта WindowsProtectionState.](../resources/intune-devices-windowsprotectionstate.md)

В следующей таблице показаны свойства, необходимые при создании [windowsProtectionState.](../resources/intune-devices-windowsprotectionstate.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для объекта защиты от устройства. Это id устройства|
|malwareProtectionEnabled|Логический|Включено или не включено вредоносное ПО|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|Состояние компьютера (например, очистка или ожидание полного сканирования или ожидающих перезагрузки и т.д.). Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|realTimeProtectionEnabled|Логический|Включена защита в режиме реального времени или нет?|
|networkInspectionSystemEnabled|Логический|Включена или нет включена система сетевого контроля?|
|quickScanOverdue|Логический|Быстрое сканирование просрочено или нет?|
|fullScanOverdue|Логический|Полная просроченная проверка или нет?|
|signatureUpdateOverdue|Логический|Подпись устарела или нет?|
|rebootRequired|Логический|Перезагрузка требуется или нет?|
|fullScanRequired|Логический|Полное сканирование требуется или нет?|
|engineVersion|Строка|Версия двигателя защиты конечной точки|
|signatureVersion|String|Текущая версия определений вредоносных программ|
|antiMalwareVersion|Строка|Текущая версия антивирусных программ|
|lastQuickScanDateTime|DateTimeOffset|Дата последнего быстрого сканирования|
|lastFullScanDateTime|DateTimeOffset|Дата последнего быстрого сканирования|
|lastQuickScanSignatureVersion|Строка|Последняя версия подписи быстрого сканирования|
|lastFullScanSignatureVersion|String|Последняя версия подписи полного сканирования|
|lastReportedDateTime|DateTimeOffset|Время последнего состояния состояния устройства|
|productStatus|[windowsDefenderProductStatus](../resources/intune-devices-windowsdefenderproductstatus.md)|Состояние продукта антивирусная программа . Возможные значения: `noStatus` `serviceNotRunning` , `serviceStartedWithoutMalwareProtection` `pendingFullScanDueToThreatAction` `pendingRebootDueToThreatAction` `pendingManualStepsDueToThreatAction` `avSignaturesOutOfDate` `asSignaturesOutOfDate` `noQuickScanHappenedForSpecifiedPeriod` `noFullScanHappenedForSpecifiedPeriod` `systemInitiatedScanInProgress` `systemInitiatedCleanInProgress` `samplesPendingSubmission` `productRunningInEvaluationMode` `productRunningInNonGenuineMode` `productExpired` `offlineScanRequired` `serviceShutdownAsPartOfSystemShutdown` `threatRemediationFailedCritically` `threatRemediationFailedNonCritically` `noStatusFlagsSet` `platformOutOfDate` `platformUpdateInProgress` `platformAboutToBeOutdated` `signatureOrPlatformEndOfLifeIsPastOrIsImpending` . `windowsSModeSignaturesInUseOnNonWin10SInstall`|
|isVirtualMachine|Логический|Указывает, является ли устройство виртуальной машиной.|
|tamperProtectionEnabled|Логический|Указывает, включена ли Защитник Windows защита от взлома.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
Content-type: application/json
Content-length: 971

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "productStatus": "serviceNotRunning",
  "isVirtualMachine": true,
  "tamperProtectionEnabled": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1020

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "productStatus": "serviceNotRunning",
  "isVirtualMachine": true,
  "tamperProtectionEnabled": true
}
```




