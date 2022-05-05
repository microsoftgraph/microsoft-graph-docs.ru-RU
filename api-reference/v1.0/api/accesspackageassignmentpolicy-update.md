---
title: Обновление accessPackageAssignmentPolicy
description: Обновление свойств объекта accessPackageAssignmentPolicy.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bacd3eb3c3e65effa389046a8d9aa1b554d5d91c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209865"
---
# <a name="update-accesspackageassignmentpolicy"></a>Обновление accessPackageAssignmentPolicy

Пространство имен: microsoft.graph


Обновите [существующий объект accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) , чтобы изменить одно или несколько его свойств, например отображаемое имя или описание.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /identityGovernance/entitlementManagement/assignmentPolicies/{accessPackageAssignmentPolicyId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя политики.|
|description|Строка|Описание политики.|
|allowedTargetScope|allowedTargetScope|Кто может запрашивать пакет доступа с помощью этой политики. Возможные значения: `notSpecified`, `specificDirectoryUsers`, `specificConnectedOrganizationUsers`, `specificDirectoryServicePrincipals`, `allMemberUsers`, `allDirectoryUsers`, `allDirectoryServicePrincipals`, `allConfiguredConnectedOrganizationUsers`, `allExternalUsers`, `unknownFutureValue`.|
|specificAllowedTargets|[Коллекция subjectSet](../resources/subjectset.md)|Субъектам, которые могут быть назначены доступ из пакета доступа с помощью этой политики.|
|Истечения срока действия|[expirationPattern](../resources/expirationpattern.md)|Дата окончания срока действия для назначений, созданных в этой политике.|
|requestorSettings|[accessPackageAssignmentRequestorSettings](../resources/accesspackageassignmentrequestorsettings.md)|Предоставляет дополнительные параметры, чтобы выбрать, кто может создать запрос на назначение пакета для доступа с помощью этой политики и что они могут включить в свой запрос.|
|requestApprovalSettings|[accessPackageAssignmentApprovalSettings](../resources/accesspackageassignmentapprovalsettings.md)|Задает параметры для утверждения запросов на назначение пакета доступа с помощью этой политики. Например, если требуется утверждение для новых запросов.|
|reviewSettings|[accessPackageReviewSettings](../resources/accesspackageassignmentreviewsettings.md)|Параметры для проверки доступа к назначениям с помощью этой политики.|

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код `200 OK` отклика и обновленный объект [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) в тексте отклика.



## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accesspackageassignmentpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentPolicies/87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187
Content-Type: application/json

{
  "id":"87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187",
  "displayName": "All Users",
  "description": "All users can request for access to the directory.",
  "allowedTargetScope": "allDirectoryUsers",
  "specificAllowedTargets": [],
  "expiration": {
      "type": "noExpiration"
  },
  "requestorSettings": {
      "enableTargetsToSelfAddAccess": true,
      "enableTargetsToSelfUpdateAccess": false,
      "enableTargetsToSelfRemoveAccess": true,
      "allowCustomAssignmentSchedule": false,
      "enableOnBehalfRequestorsToAddAccess": false,
      "enableOnBehalfRequestorsToUpdateAccess": false,
      "enableOnBehalfRequestorsToRemoveAccess": false,
      "onBehalfRequestors": []
  },
  "requestApprovalSettings": {
      "isApprovalRequiredForAdd": true,
      "isApprovalRequiredForUpdate": false,
      "stages": [
          {
              "durationBeforeAutomaticDenial": "P2D",
              "isApproverJustificationRequired": false,
              "isEscalationEnabled": false,
              "durationBeforeEscalation": "PT0S",
              "primaryApprovers": [
                  {
                      "@odata.type": "#microsoft.graph.requestorManager",
                      "managerLevel": 1
                  }
              ],
              "fallbackPrimaryApprovers": [
                  {
                      "@odata.type": "#microsoft.graph.singleUser",
                      "userId": "e6bf4d7d-6824-4dd0-809d-5bf42d4817c2",
                      "description": "user"
                  }
              ],
              "escalationApprovers": [],
              "fallbackEscalationApprovers": []
          }
      ]
  },
  "accessPackage": {
        "id": "49d2c59b-0a81-463d-a8ec-ddad3935d8a0"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accesspackageassignmentpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187",
  "displayName": "All Users",
  "description": "All users can request for access to the directory."
}
```

