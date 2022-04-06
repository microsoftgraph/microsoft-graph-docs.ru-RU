---
title: Создание assignmentPolicies
description: Создание нового объекта accessPackageAssignmentPolicy.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 848f259c6d40ae14fb45c9230ad4d0b524dbf17b
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608376"
---
# <a name="create-assignmentpolicies"></a>Создание assignmentPolicies
Пространство имен: microsoft.graph

В [управлении правами Azure AD](../resources/entitlementmanagement-overview.md) создайте новый [объект accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .  Запрос будет содержать ссылку на [accessPackage](../resources/accesspackage.md) , которая будет содержать эту политику, которая уже должна существовать.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.ReadWrite.All  |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | EntitlementManagement.ReadWrite.All |


## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/assignmentPolicies
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON объекта [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) .

При создании **accessPackageAssignmentPolicy** можно указать следующие свойства.

|Свойство|Тип|Описание|
|:---|:---|:---|
|description|Строка|Описание политики.|
|displayName|Строка|Отображает имя политики.|
|allowedTargetScope|allowedTargetScope|Кто может быть назначен пакет доступа через эту политику. Возможные значения: `notSpecified`, `specificDirectoryUsers`, `specificConnectedOrganizationUsers`, `specificDirectoryServicePrincipals`, `allMemberUsers`, `allDirectoryUsers`, `allDirectoryServicePrincipals`, `allConfiguredConnectedOrganizationUsers`, `allExternalUsers`, `unknownFutureValue`. Необязательно.|
|истечение срока действия|[expirationPattern](../resources/expirationpattern.md)|Срок действия для назначений, созданных в этой политике.|
|requestApprovalSettings|[accessPackageAssignmentApprovalSettings](../resources/accesspackageassignmentapprovalsettings.md)|Указывает параметры для утверждения запросов на назначение пакета доступа с помощью этой политики. Например, если требуется утверждение для новых запросов.|
|requestorSettings|[accessPackageAssignmentRequestorSettings](../resources/accesspackageassignmentrequestorsettings.md)|Предоставляет дополнительные параметры, чтобы выбрать, кто может создать запрос на назначение пакета доступа с помощью этой политики и что они могут включить в свой запрос.|
|specificAllowedTargets|[коллекция subjectSet](../resources/subjectset.md)|Целевые показатели для получения доступа из пакета доступа из этой политики.|
|accessPackage|[accessPackage](../resources/accesspackage.md)| Ссылка на пакет доступа, который будет содержать политику, которая уже должна существовать.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот `201 Created` метод возвращает код отклика и [объект accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/assignmentPolicies
Content-Type: application/json

{
  "displayName": "New Policy",
  "description": "policy for assignment",
  "allowedTargetScope": "notSpecified",
  "specificAllowedTargets": [],
  "expiration": {
      "endDateTime": null,
      "duration": null,
      "type": "noExpiration"
  },
  "requestorSettings": {
      "enableTargetsToSelfAddAccess": false,
      "enableTargetsToSelfUpdateAccess": false,
      "enableTargetsToSelfRemoveAccess": false,
      "allowCustomAssignmentSchedule": true,
      "enableOnBehalfRequestorsToAddAccess": false,
      "enableOnBehalfRequestorsToUpdateAccess": false,
      "enableOnBehalfRequestorsToRemoveAccess": false,
      "onBehalfRequestors": []
  },
  "requestApprovalSettings": {
      "isApprovalRequiredForAdd": false,
      "isApprovalRequiredForUpdate": false,
      "stages": []
  },
  "accessPackage": {
      "id": "a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b"
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
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187",
  "displayName": "New policy",
  "description": "policy for assignment"
}
```


