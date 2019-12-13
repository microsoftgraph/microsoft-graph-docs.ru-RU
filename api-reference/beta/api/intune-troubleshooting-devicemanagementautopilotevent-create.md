---
title: Создание Девицеманажементаутопилотевент
description: Создание нового объекта Девицеманажементаутопилотевент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1db911f6f1386c4244703c4fb422ecfeb44e0232
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939045"
---
# <a name="create-devicemanagementautopilotevent"></a>Создание Девицеманажементаутопилотевент

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта Девицеманажементаутопилотевент в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Девицеманажементаутопилотевент.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|UUID объекта.|
|eventDateTime|DateTimeOffset|Время возникновения события.|
|девицерегистереддатетиме|DateTimeOffset|Дата регистрации устройства.|
|енроллментстартдатетиме|DateTimeOffset|Дата начала регистрации устройства.|
|enrollmentType|[windowsAutopilotEnrollmentType](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|Тип регистрации. Возможные значения: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.|
|девицесериалнумбер|Строка|Серийный номер устройства.|
|managedDeviceName|String|Управляемое имя устройства.|
|userPrincipalName|String|Имя участника пользователя, используемое для регистрации устройства.|
|виндовсаутопилотдеплойментпрофиледисплайнаме|Строка|Имя профиля для автопилота.|
|енроллментстате|[енроллментстате](../resources/intune-shared-enrollmentstate.md)|Не удалось зарегистрировать состояние регистрации, например "зарегистрировано". Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|windows10EnrollmentCompletionPageConfigurationDisplayName|Строка|Имя профиля страницы состояния регистрации|
|деплойментстате|[windowsAutopilotDeploymentState](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|Состояние развертывания, например успешное выполнение, сбой, выполнение, Сукцессвистимеаут. Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`.|
|osVersion|Строка|Версия операционной системы устройства.|
|деплойментдуратион|Длительность|Длительность развертывания с автопилотной версией, включая регистрацию.|
|деплойменттоталдуратион|Длительность|Общее время развертывания с экрана регистрации на рабочем столе.|
|девицепрепаратиондуратион|Длительность|Время, затраченное на регистрацию устройств.|
|девицесетупдуратион|Длительность|Время, затраченное на устройство ESP.|
|аккаунтсетупдуратион|Длительность|Время, затраченное на ESP пользователем.|
|деплойментстартдатетиме|DateTimeOffset|Время начала развертывания.|
|деплойментенддатетиме|DateTimeOffset|Время окончания развертывания.|
|таржетедаппкаунт|Int32|Количество целевых приложений.|
|таржетедполицикаунт|Int32|Количество целевых политик.|
|енроллментфаилуредетаилс|Строка|Сведения о сбоях при регистрации.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементаутопилотевент](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents
Content-type: application/json
Content-length: 1323

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "deviceRegisteredDateTime": "2017-01-01T00:02:48.7185581-08:00",
  "enrollmentStartDateTime": "2017-01-01T00:00:19.6280481-08:00",
  "enrollmentType": "azureADJoinedWithAutopilotProfile",
  "deviceSerialNumber": "Device Serial Number value",
  "managedDeviceName": "Managed Device Name value",
  "userPrincipalName": "User Principal Name value",
  "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
  "enrollmentState": "enrolled",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
  "deploymentState": "success",
  "osVersion": "Os Version value",
  "deploymentDuration": "PT3M21.5549443S",
  "deploymentTotalDuration": "PT1M43.5284261S",
  "devicePreparationDuration": "-PT1M32.1347897S",
  "deviceSetupDuration": "-PT2M57.2190107S",
  "accountSetupDuration": "-PT2M32.0507894S",
  "deploymentStartDateTime": "2016-12-31T23:59:37.257201-08:00",
  "deploymentEndDateTime": "2017-01-01T00:00:46.5128291-08:00",
  "targetedAppCount": 0,
  "targetedPolicyCount": 3,
  "enrollmentFailureDetails": "Enrollment Failure Details value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1372

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "3e455cab-5cab-3e45-ab5c-453eab5c453e",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "deviceRegisteredDateTime": "2017-01-01T00:02:48.7185581-08:00",
  "enrollmentStartDateTime": "2017-01-01T00:00:19.6280481-08:00",
  "enrollmentType": "azureADJoinedWithAutopilotProfile",
  "deviceSerialNumber": "Device Serial Number value",
  "managedDeviceName": "Managed Device Name value",
  "userPrincipalName": "User Principal Name value",
  "windowsAutopilotDeploymentProfileDisplayName": "Windows Autopilot Deployment Profile Display Name value",
  "enrollmentState": "enrolled",
  "windows10EnrollmentCompletionPageConfigurationDisplayName": "Windows10Enrollment Completion Page Configuration Display Name value",
  "deploymentState": "success",
  "osVersion": "Os Version value",
  "deploymentDuration": "PT3M21.5549443S",
  "deploymentTotalDuration": "PT1M43.5284261S",
  "devicePreparationDuration": "-PT1M32.1347897S",
  "deviceSetupDuration": "-PT2M57.2190107S",
  "accountSetupDuration": "-PT2M32.0507894S",
  "deploymentStartDateTime": "2016-12-31T23:59:37.257201-08:00",
  "deploymentEndDateTime": "2017-01-01T00:00:46.5128291-08:00",
  "targetedAppCount": 0,
  "targetedPolicyCount": 3,
  "enrollmentFailureDetails": "Enrollment Failure Details value"
}
```





