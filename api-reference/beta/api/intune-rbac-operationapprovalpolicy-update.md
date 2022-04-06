---
title: Обновление операцииApprovalPolicy
description: Обновление свойств объекта operationApprovalPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1d64af17564bbdb8612814576b6190ef7d741716
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2022
ms.locfileid: "64630886"
---
# <a name="update-operationapprovalpolicy"></a>Обновление операцииApprovalPolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementRBAC.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementRBAC.ReadWrite.All|

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
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) .

В следующей таблице показаны свойства, необходимые при создании [операцииApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ID операцииApprovalPolicy. Это свойство доступно только для чтения.|
|displayName|Строка|Имя отображения этой операцииApprovalPolicy|
|description|Строка|Описание этой операцииApprovalPolicy|
|lastModifiedDateTime|DateTimeOffset|Последняя измененная дата и время операцииApprovalPolicy. Это свойство доступно только для чтения.|
|policyType|[operationApprovalPolicyType](../resources/intune-rbac-operationapprovalpolicytype.md)|Тип политики для этой операцииApprovalPolicy. Возможные значения: `deviceActions`, `deviceWipe`, `deviceRetire`, `deviceRetireNonCompliant`, `deviceDelete`, `deviceLock`, `apps``windowsEnrollment``compliancePolicies``deviceDisableActivationLock``configurationPolicies``endpointSecurity``policySets``appProtectionPolicies``deviceErase``scripts``roles``filters`, . `unknownFutureValue``deviceResetPasscode`|
|approverGroupIds|Коллекция объектов string|Групповые ID для тех, кто одобряет эту операциюApprovalPolicy|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код `200 OK` ответа и обновленный объект [operationApprovalPolicy](../resources/intune-rbac-operationapprovalpolicy.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/operationApprovalPolicies/{operationApprovalPolicyId}
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.operationApprovalPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "policyType": "deviceWipe",
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
Content-Length: 351

{
  "@odata.type": "#microsoft.graph.operationApprovalPolicy",
  "id": "9d2caa5f-aa5f-9d2c-5faa-2c9d5faa2c9d",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "policyType": "deviceWipe",
  "approverGroupIds": [
    "Approver Group Ids value"
  ]
}
```




