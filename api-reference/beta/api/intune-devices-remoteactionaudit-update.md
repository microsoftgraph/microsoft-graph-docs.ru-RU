---
title: Обновление remoteActionAudit
description: Обновление свойств объекта remoteActionAudit.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02c2af28995b72246bc82f7af8d27e1f1171adc0
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51609502"
---
# <a name="update-remoteactionaudit"></a>Обновление remoteActionAudit

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
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
PATCH /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)

В следующей таблице показаны свойства, необходимые при создании [remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Report Id.|
|deviceDisplayName|String|Имя устройства Intune.|
|userName|String|\[deprecated \] Please use InitiatedByUserPrincipalName instead.|
|initiatedByUserPrincipalName|String|Пользователь, который инициировал действие устройства, формат upN.|
|action|[remoteAction](../resources/intune-devices-remoteaction.md)|Имя действия. Возможные значения: `unknown` `factoryReset` , , `removeCompanyData` `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` , `quickScan` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey` `getFileVaultKey` `setDeviceName` .|
|requestDateTime|DateTimeOffset|Время, когда действие было выдано, дано в UTC.|
|deviceOwnerUserPrincipalName|String|Upn владельца устройства.|
|deviceIMEI|String|IMEI устройства.|
|actionState|[actionState](../resources/intune-devices-actionstate.md)|Состояние действия. Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|managedDeviceId|String|Цель действия.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
Content-type: application/json
Content-length: 504

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending",
  "managedDeviceId": "Managed Device Id value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending",
  "managedDeviceId": "Managed Device Id value"
}
```




