---
title: Обновление windowsProtectionState
description: Обновление свойств объекта windowsProtectionState.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 593ba645ef109742c295c3f45bb2c2e4d3af3be6
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790555"
---
# <a name="update-windowsprotectionstate"></a>Обновление windowsProtectionState

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementManagedDevices.ReadWrite.All|

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
В тексте запроса добавьте представление объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для объекта состояния защиты устройства. Это идентификатор устройства для устройства.|
|малварепротектионенаблед|Логический|Защита от вредоносных программ включена или нет|
|девицестате|[виндовсдевицехеалсстате](../resources/intune-devices-windowsdevicehealthstate.md)|Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.). Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|реалтимепротектионенаблед|Логический|Защита в режиме реального времени включена или нет?|
|нетворкинспектионсистеменаблед|Логический|Система проверки сети включена или нет?|
|куиккскановердуе|Логический|Быстрая проверка просрочена или нет?|
|фуллскановердуе|Логический|Полная проверка просрочена или нет?|
|сигнатуреупдатеовердуе|Логический|Подпись устарела или нет?|
|ребутрекуиред|Логический|Требуется перезагрузка или нет?|
|фуллсканрекуиред|Логический|Необходима полная проверка или нет?|
|енгиневерсион|String|Текущая версия модуля Endpoint Protection|
|сигнатуреверсион|String|Текущая версия определений вредоносных программ|
|антималвареверсион|String|Текущая версия защиты от вредоносных программ|
|ласткуиккскандатетиме|DateTimeOffset|Дата и время последнего быстрого сканирования|
|ластфуллскандатетиме|DateTimeOffset|Дата и время последнего быстрого сканирования|
|ласткуиккскансигнатуреверсион|String|Последняя версия подписи быстрого сканирования|
|ластфуллскансигнатуреверсион|String|Версия последней полной проверки подписи|
|lastReportedDateTime|DateTimeOffset|Последнее состояние работоспособности устройства в отчете о времени|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
Content-type: application/json
Content-length: 865

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
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

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
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```



