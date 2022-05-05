---
title: Создание operationApprovalRequest
description: Создайте объект operationApprovalRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2d279732025e39af5081104832138b542c68ba52
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210852"
---
# <a name="create-operationapprovalrequest"></a>Создание operationApprovalRequest

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте объект [operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementRBAC.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementRBAC.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/operationApprovalRequests
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта operationApprovalRequest в формате JSON.

В следующей таблице показаны свойства, необходимые при создании operationApprovalRequest.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор сущности|
|requestDateTime|DateTimeOffset|DateTime запроса. Это свойство доступно только для чтения.|
|expirationDateTime|DateTimeOffset|Дата и время, когда действия по запросу больше не разрешены. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения. Это свойство доступно только для чтения.|
|Запрашивающего|[identitySet](../resources/intune-rbac-identityset.md)|Удостоверение запрашиваемого объекта. Это свойство доступно только для чтения.|
|Утверждающий|[identitySet](../resources/intune-rbac-identityset.md)|Удостоверение утверждающего. Это свойство доступно только для чтения.|
|status|[operationApprovalRequestStatus](../resources/intune-rbac-operationapprovalrequeststatus.md)|Текущее состояние запроса на утверждение. Это свойство доступно только для чтения. Возможные значения: `unknown`, `needsApproval`, `approved`, `rejected`, `cancelled`, `completed`, `expired`, `unknownFutureValue`.|
|requestJustification|Строка|Обоснование запроса. Это свойство доступно только для чтения.|
|approvalJustification|Строка|Обоснование утверждения запроса. Это свойство доступно только для чтения.|
|operationApprovalPolicies|Строка|Политики рабочего утверждения, используемые в запросе. Это свойство доступно только для чтения.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код `201 Created` отклика и объект [operationApprovalRequest](../resources/intune-rbac-operationapprovalrequest.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/operationApprovalRequests
Content-type: application/json
Content-length: 1415

{
  "@odata.type": "#microsoft.graph.operationApprovalRequest",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "requestor": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  },
  "approver": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  },
  "status": "needsApproval",
  "requestJustification": "Request Justification value",
  "approvalJustification": "Approval Justification value",
  "operationApprovalPolicies": "Operation Approval Policies value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1528

{
  "@odata.type": "#microsoft.graph.operationApprovalRequest",
  "id": "4e9eed82-ed82-4e9e-82ed-9e4e82ed9e4e",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "requestor": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  },
  "approver": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  },
  "status": "needsApproval",
  "requestJustification": "Request Justification value",
  "approvalJustification": "Approval Justification value",
  "operationApprovalPolicies": "Operation Approval Policies value"
}
```




