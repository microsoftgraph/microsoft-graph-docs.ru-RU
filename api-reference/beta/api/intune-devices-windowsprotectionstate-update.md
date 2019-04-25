---
title: Обновление windowsProtectionState
description: Обновление свойств объекта windowsProtectionState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b53e93f09be2b091ffe3e6a30cd109feb55c8d8a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534292"
---
# <a name="update-windowsprotectionstate"></a>Обновление windowsProtectionState

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для объекта состояния защиты устройства. Это идентификатор устройства для устройства.|
|Малварепротектионенаблед|Логический|Защита от вредоносных программ включена или нет|
|Девицестате|[Виндовсдевицехеалсстате](../resources/intune-devices-windowsdevicehealthstate.md)|Состояние компьютера (например, очистка или ожидание полного сканирования или Ожидание перезагрузки и т. д.). Возможные значения: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.|
|Реалтимепротектионенаблед|Логический|Защита в режиме реального времени включена или нет?|
|Нетворкинспектионсистеменаблед|Логический|Система проверки сети включена или нет?|
|Куиккскановердуе|Логический|Быстрая проверка просрочена или нет?|
|Фуллскановердуе|Логический|Полная проверка просрочена или нет?|
|Сигнатуреупдатеовердуе|Логический|Подпись устарела или нет?|
|Ребутрекуиред|Логический|Требуется переЗагрузка или нет?|
|Фуллсканрекуиред|Логический|Необходима полная проверка или нет?|
|Енгиневерсион|String|Текущая версия модуля Endpoint Protection|
|Сигнатуреверсион|String|Текущая версия определений вредоносных программ|
|Антималвареверсион|String|Текущая версия защиты от вредоносных программ|
|Ласткуиккскандатетиме|DateTimeOffset|Дата и время последнего быстрого сканирования|
|Ластфуллскандатетиме|DateTimeOffset|Дата и время последнего быстрого сканирования|
|Ласткуиккскансигнатуреверсион|String|Последняя версия подписи быстрого сканирования|
|Ластфуллскансигнатуреверсион|String|Версия последней полной проверки подписи|
|lastReportedDateTime|DateTimeOffset|Последнее состояние работоспособности устройства в отчете о времени|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
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
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
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





