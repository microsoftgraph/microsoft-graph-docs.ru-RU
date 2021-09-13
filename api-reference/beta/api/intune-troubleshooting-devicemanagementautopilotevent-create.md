---
title: Создание deviceManagementAutopilotEvent
description: Создание нового объекта deviceManagementAutopilotEvent.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d1197d1a542df099243a00d989c25273db124a07
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59116173"
---
# <a name="create-devicemanagementautopilotevent"></a>Создание deviceManagementAutopilotEvent

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта deviceManagementAutopilotEvent.](../resources/intune-troubleshooting-devicemanagementautopilotevent.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
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
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта deviceManagementAutopilotEvent.

В следующей таблице показаны свойства, необходимые при создании устройстваManagementAutopilotEvent.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|UUID объекта.|
|deviceId|String|ID устройства, связанный с объектом|
|eventDateTime|DateTimeOffset|Время возникновения события.|
|deviceRegisteredDateTime|DateTimeOffset|Дата регистрации устройства.|
|enrollmentStartDateTime|DateTimeOffset|Дата начала регистрации устройства.|
|enrollmentType|[windowsAutopilotEnrollmentType](../resources/intune-troubleshooting-windowsautopilotenrollmenttype.md)|Тип регистрации. Возможные значения: `unknown`, `azureADJoinedWithAutopilotProfile`, `offlineDomainJoined`, `azureADJoinedUsingDeviceAuthWithAutopilotProfile`, `azureADJoinedUsingDeviceAuthWithoutAutopilotProfile`, `azureADJoinedWithOfflineAutopilotProfile`, `azureADJoinedWithWhiteGlove`, `offlineDomainJoinedWithWhiteGlove`, `offlineDomainJoinedWithOfflineAutopilotProfile`.|
|deviceSerialNumber|String|Серийный номер устройства.|
|managedDeviceName|String|Имя управляемого устройства.|
|userPrincipalName|String|Имя пользователя, используемая для регистрации устройства.|
|windowsAutopilotDeploymentProfileDisplayName|String|Имя профиля автопилота.|
|enrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Состояние регистрации, как "Регистрация", "Сбой". Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|windows10EnrollmentCompletionPageConfigurationDisplayName|String|Имя профиля страницы состояния регистрации|
|windows10EnrollmentCompletionPageConfigurationId|String|ID профиля страницы состояния регистрации|
|deploymentState|[windowsAutopilotDeploymentState](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|Состояние развертывания, такое как Success, Failure, InProgress, SuccessWithTimeout. Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.|
|deviceSetupStatus|[windowsAutopilotDeploymentState](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|Состояние развертывания для этапа установки устройства состояния страницы регистрации. Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.|
|accountSetupStatus|[windowsAutopilotDeploymentState](../resources/intune-troubleshooting-windowsautopilotdeploymentstate.md)|Состояние развертывания для этапа настройки учетной записи страницы состояния регистрации. Возможные значения: `unknown`, `success`, `inProgress`, `failure`, `successWithTimeout`, `notAttempted`, `disabled`.|
|osVersion|String|Версия операционной системы устройства.|
|deploymentDuration|Длительность|Продолжительность развертывания автопилота, включая регистрацию.|
|deploymentTotalDuration|Длительность|Общая продолжительность развертывания от регистрации до экрана Desktop.|
|devicePreparationDuration|Длительность|Время, затраченное на регистрацию устройств.|
|deviceSetupDuration|Длительность|Время, проведенное в устройстве ESP.|
|accountSetupDuration|Длительность|Время, затраченное в пользовательском ESP.|
|deploymentStartDateTime|DateTimeOffset|Время начала развертывания.|
|deploymentEndDateTime|DateTimeOffset|Время окончания развертывания.|
|targetedAppCount|Int32|Количество целевых приложений.|
|targetedPolicyCount|Int32|Количество целевых политик.|
|enrollmentFailureDetails|String|Сведения о сбое регистрации.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementAutopilotEvent](../resources/intune-troubleshooting-devicemanagementautopilotevent.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/v1/deviceManagement/autopilotEvents
Content-type: application/json
Content-length: 1545

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "deviceId": "Device Id value",
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
  "windows10EnrollmentCompletionPageConfigurationId": "Windows10Enrollment Completion Page Configuration Id value",
  "deploymentState": "success",
  "deviceSetupStatus": "success",
  "accountSetupStatus": "success",
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
Content-Length: 1594

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotEvent",
  "id": "3e455cab-5cab-3e45-ab5c-453eab5c453e",
  "deviceId": "Device Id value",
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
  "windows10EnrollmentCompletionPageConfigurationId": "Windows10Enrollment Completion Page Configuration Id value",
  "deploymentState": "success",
  "deviceSetupStatus": "success",
  "accountSetupStatus": "success",
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




