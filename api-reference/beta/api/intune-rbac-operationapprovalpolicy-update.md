---
title: Обновление операцииApprovalPolicy
description: Обновление свойств объекта operationApprovalPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 499c1122cf40ef5c4340f978a29f56995b8a2af4
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60487434"
---
# <a name="update-operationapprovalpolicy"></a>Обновление операцииApprovalPolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [operationApprovalPolicy.](../resources/intune-rbac-operationapprovalpolicy.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementRBAC.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementRBAC.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/operationApprovalPolicies/{operationApprovalPolicyId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта operationApprovalPolicy.](../resources/intune-rbac-operationapprovalpolicy.md)

В следующей таблице показаны свойства, необходимые при создании [операцииApprovalPolicy.](../resources/intune-rbac-operationapprovalpolicy.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID операцииApprovalPolicy. Это свойство доступно только для чтения.|
|displayName|String|Имя отображения этой операцииApprovalPolicy|
|description|String|Описание этой операцииApprovalPolicy|
|lastModifiedDateTime|DateTimeOffset|Последняя измененная дата и время операцииApprovalPolicy. Это свойство доступно только для чтения.|
|policyType|[operationApprovalPolicyType](../resources/intune-rbac-operationapprovalpolicytype.md)|Тип политики для этой операцииApprovalPolicy. Возможные значения: `deviceActions` `deviceWipe` , , , , , `deviceRetire` , , , `deviceRetireNonCompliant` `deviceDelete` , , `deviceLock` `deviceErase` `deviceDisableActivationLock` `windowsEnrollment` , `compliancePolicies` `configurationPolicies` `appProtectionPolicies` `policySets` `filters` `endpointSecurity` `apps` `scripts` `roles` `unknownFutureValue` .|
|policyPlatform|[operationApprovalPolicyPlatform](../resources/intune-rbac-operationapprovalpolicyplatform.md)|Применимая платформа (ы) для этой ОперацииApprovalPolicy. Возможные значения: `notApplicable`, `androidDeviceAdministrator`, `androidEnterprise`, `iOSiPadOS`, `macOS`, `windows10AndLater`, `windows81AndLater`, `windows10X`.|
|approverGroupIds|Коллекция строк|Групповые ID для тех, кто одобряет эту операциюApprovalPolicy|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/operationApprovalPolicies/{operationApprovalPolicyId}
Content-type: application/json
Content-length: 289

{
  "@odata.type": "#microsoft.graph.operationApprovalPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "policyType": "deviceWipe",
  "policyPlatform": "androidDeviceAdministrator",
  "approverGroupIds": [
    "Approver Group Ids value"
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 402

{
  "@odata.type": "#microsoft.graph.operationApprovalPolicy",
  "id": "9d2caa5f-aa5f-9d2c-5faa-2c9d5faa2c9d",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "policyType": "deviceWipe",
  "policyPlatform": "androidDeviceAdministrator",
  "approverGroupIds": [
    "Approver Group Ids value"
  ]
}
```



