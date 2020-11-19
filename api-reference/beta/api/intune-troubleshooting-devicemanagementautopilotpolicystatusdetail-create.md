---
title: Создание Девицеманажементаутопилотполицистатусдетаил
description: Создание нового объекта Девицеманажементаутопилотполицистатусдетаил.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5a4a1680ec58e52d920a1cea8bf6772974bbb8f7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299928"
---
# <a name="create-devicemanagementautopilotpolicystatusdetail"></a>Создание Девицеманажементаутопилотполицистатусдетаил

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .

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
POST /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта Девицеманажементаутопилотполицистатусдетаил в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Девицеманажементаутопилотполицистатусдетаил.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|UUID объекта.|
|displayName|String|Понятное имя политики.|
|полицитипе|[deviceManagementAutopilotPolicyType](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|Тип политики. Возможные значения: `unknown`, `application`, `appModel`, `configurationPolicy`.|
|комплианцестатус|[deviceManagementAutopilotPolicyComplianceStatus](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|Состояние соответствия политике. Возможные значения: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.|
|траккедоненроллментстатус|Boolean|Указывает, была ли эта пролици зарегистрирована в рамках сеанса синхронизации автоматической загрузки для автоматической пилотной установки|
|lastReportedDateTime|DateTimeOffset|Метка времени для отчета о состоянии политики|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
Content-type: application/json
Content-length: 295

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "displayName": "Display Name value",
  "policyType": "application",
  "complianceStatus": "compliant",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 344

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "id": "dbe093ee-93ee-dbe0-ee93-e0dbee93e0db",
  "displayName": "Display Name value",
  "policyType": "application",
  "complianceStatus": "compliant",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```




