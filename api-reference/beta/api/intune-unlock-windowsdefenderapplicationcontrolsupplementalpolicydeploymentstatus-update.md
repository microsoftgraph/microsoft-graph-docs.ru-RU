---
title: Обновление windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus
description: Обновление свойств объекта WindowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ca2c178687cdee7cca180b3c453ce152511b0c6c8f3d421ec319bfee216a176
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54210430"
---
# <a name="update-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"></a>Обновление windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [WindowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В корпусе запроса поставляем представление JSON для [объекта WindowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)

В следующей таблице показаны свойства, необходимые при создании [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus.](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|deviceName|String|Имя устройства.|
|deviceId|String|ID устройства.|
|lastSyncDateTime|DateTimeOffset|Дата последней синхронизации.|
|osVersion|String|Windows ВЕРСИЯ ОС.|
|osDescription|String|Windows Описание версии ОС.|
|deploymentStatus|[windowsDefenderApplicationControlSupplementalPolicyStatuses](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicystatuses.md)|Состояние развертывания политики. Возможные значения: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.|
|userName|String|Имя пользователя этого устройства.|
|userPrincipalName|String|Имя главного пользователя.|
|policyVersion|String|Человеческая читаемая версия дополнительной политики WindowsDefenderApplicationControl.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект WindowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/intune-unlock-windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
Content-type: application/json
Content-length: 486

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "deploymentStatus": "success",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "policyVersion": "Policy Version value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 535

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
  "id": "e3c01841-1841-e3c0-4118-c0e34118c0e3",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "deploymentStatus": "success",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "policyVersion": "Policy Version value"
}
```




