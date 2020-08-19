---
title: Обновление Акцесспаккажеассигнментполици
description: Обновление свойств объекта Акцесспаккажеассигнментполици.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 086bc79bf6462d569f85e4abf885a8c8538356ae
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806428"
---
# <a name="update-accesspackageassignmentpolicy"></a>Обновление Акцесспаккажеассигнментполици

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление существующего объекта [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) для изменения одного или нескольких его свойств, таких как отображаемое имя или описание.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
```http
PUT /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{accessPackageAssignmentPolicyId}
```
## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при обновлении [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя политики.|
|description|String|Описание политики.|
|canExtend|Логический|Указывает, может ли пользователь продлить продолжительность назначения пакета доступа после утверждения.|
|дуратиониндайс|Int32|Количество дней, в течение которых назначения из этой политики последний раз до истечения срока действия.|
|expirationDateTime|DateTimeOffset|Срок действия для назначений, созданных в этой политике. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|рекуесторсеттингс|[рекуесторсеттингс](../resources/requestorsettings.md)|Кто может запрашивать этот пакет Access из этой политики.|
|рекуестаппровалсеттингс|[аппровалсеттингс](../resources/approvalsettings.md)|Кто должен утверждать запросы на пакет Access в этой политике.|
|акцессревиевсеттингс|[ассигнментревиевсеттингс](../resources/assignmentreviewsettings.md)|Кто должен проверить и как часто назначений для пакета доступа из этой политики. Это свойство имеет значение null, если проверка не требуются.|


## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md) в тексте отклика.



## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accesspackageassignmentpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/b2eba9a1-b357-42ee-83a8-336522ed6cbf
Content-Type: application/json
Content-length: 1000

{
  "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
  "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
  "displayName": "All Users",
  "description": "All users can request for access to the directory.",
  "isDenyPolicy": false,
  "canExtend": false,
  "durationInDays": 365,
  "requestorSettings" : {
    "scopeType": "AllExistingDirectorySubjects",
    "acceptRequests": true,
    "allowedRequestors": []
  },
  "requestApprovalSettings" : {
    "isApprovalRequired": false,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": false,
    "approvalMode": "NoApproval",
    "approvalStages": []
  },
  "accessReviewSettings" : null
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
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
  "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
  "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
  "displayName": "All Users",
  "description": "All users can request for access to the directory.",
  "isDenyPolicy": false,
  "canExtend": false,
  "durationInDays": 365,
  "accessReviewSettings" : null
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
