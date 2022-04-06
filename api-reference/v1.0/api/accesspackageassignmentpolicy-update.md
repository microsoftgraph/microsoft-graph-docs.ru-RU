---
title: Обновление accessPackageAssignmentPolicy
description: Обновление свойств объекта accessPackageAssignmentPolicy.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9721e20954105efde2c43be33ec47889884405e7
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608309"
---
# <a name="update-accesspackageassignmentpolicy"></a>Обновление accessPackageAssignmentPolicy

Пространство имен: microsoft.graph


Обнови [существующий объект accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) , чтобы изменить одно или несколько его свойств, например имя или описание отображения.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | EntitlementManagement.ReadWrite.All |

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
|displayName|String|Отображает имя политики.|
|description|Строка|Описание политики.|
|allowedTargetScope|allowedTargetScope|Кто может запрашивать пакет доступа через эту политику. Возможные значения: `notSpecified`, `specificDirectoryUsers`, `specificConnectedOrganizationUsers`, `specificDirectoryServicePrincipals`, `allMemberUsers`, `allDirectoryUsers`, `allDirectoryServicePrincipals`, `allConfiguredConnectedOrganizationUsers`, `allExternalUsers`, `unknownFutureValue`.|
|specificAllowedTargets|[коллекция subjectSet](../resources/subjectset.md)|Принципы, которые могут быть назначены доступ из пакета доступа через эту политику.|
|истечение срока действия|[expirationPattern](../resources/expirationpattern.md)|Срок действия для назначений, созданных в этой политике.|
|requestorSettings|[accessPackageAssignmentRequestorSettings](../resources/accesspackageassignmentrequestorsettings.md)|Предоставляет дополнительные параметры, чтобы выбрать, кто может создать запрос на назначение пакета доступа с помощью этой политики и что они могут включить в свой запрос.|
|requestApprovalSettings|[accessPackageAssignmentApprovalSettings](../resources/accesspackageassignmentapprovalsettings.md)|Указывает параметры для утверждения запросов на назначение пакета доступа с помощью этой политики. Например, если требуется утверждение для новых запросов.|
|reviewSettings|[accessPackageReviewSettings](../resources/accesspackageassignmentreviewsettings.md)|Параметры для проверки доступа к назначениям с помощью этой политики.|

## <a name="response"></a>Отклик
В случае успешного `200 OK` выполнения этот метод возвращает код ответа и обновленный [объект accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) в тексте ответа.



## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
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
  "accessPackage": {
        "id": "49d2c59b-0a81-463d-a8ec-ddad3935d8a0"
  }
}
```


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

