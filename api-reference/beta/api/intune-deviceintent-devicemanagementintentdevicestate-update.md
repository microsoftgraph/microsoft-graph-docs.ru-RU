---
title: Обновление Девицеманажементинтентдевицестате
description: Обновление свойств объекта Девицеманажементинтентдевицестате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b3a5c7fa45c60d70a70966f1d0210994c9a44a17
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48689589"
---
# <a name="update-devicemanagementintentdevicestate"></a>Обновление Девицеманажементинтентдевицестате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор|
|userPrincipalName|String|Имя участника-пользователя, сообщаемое на устройстве|
|userName|String|Имя пользователя, сообщаемое на устройстве|
|deviceDisplayName|String|Имя устройства, о котором сообщается|
|lastReportedDateTime|DateTimeOffset|Дата и время последнего изменения отчета о намерениях|
|state|[комплианцестатус](../resources/intune-shared-compliancestatus.md)|Состояние устройства для цели. Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|deviceId|String|Идентификатор устройства, о котором сообщается|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентдевицестате](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates/{deviceManagementIntentDeviceStateId}
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceDisplayName": "Device Display Name value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable",
  "deviceId": "Device Id value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "id": "8db75881-5881-8db7-8158-b78d8158b78d",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceDisplayName": "Device Display Name value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable",
  "deviceId": "Device Id value"
}
```





