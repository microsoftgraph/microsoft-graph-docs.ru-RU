---
title: Создание Акцесспаккажеассигнментрекуест
description: Создание нового Акцесспаккажеассигнментрекуест.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 371ab27fd9793a315b8518e0c81a30e14a4a674b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983840"
---
# <a name="create-accesspackageassignmentrequest"></a>Создание Акцесспаккажеассигнментрекуест

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении обслуживанием Azure AD](../resources/entitlementmanagement-root.md)создайте новый объект [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) .  Эта операция используется для назначения пользователя в пакет Access или для удаления назначения пакета Access.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Authorization | Носитель \{токен\}. Обязательно. |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в формате JSON.

Чтобы администратор запрашивал создание назначения для пользователя, свойство **requestType** имеет значение `AdminAdd` , а свойство **акцесспаккажеассигнмент** содержит `targetId` назначенного пользователя, свойство **ассигнментполициид** , идентифицирующее [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md), и свойство **акцесспаккажеид** , определяющее [accessPackage](../resources/accesspackage.md).

Чтобы администратор запрашивал удаление назначения, свойство **requestType** имеет значение `AdminRemove` , а свойство **акцесспаккажеассигнмент** содержит свойство **ID** , идентифицирующее удаляемое [акцесспаккажеассигнмент](../resources/accesspackageassignment.md) .

Чтобы пользователь, не являющийся администратором, запрашивался для самостоятельного создания назначения, используется значение свойства **requestType** `UserAdd` , а свойство **акцесспаккажеассигнмент** содержит `targetId` идентификатор самих пользователей, свойство **ассигнментполициид** , идентифицирующее [акцесспаккажеассигнментполици](../resources/accesspackageassignmentpolicy.md), и свойство **акцесспаккажеид** , определяющее [accessPackage](../resources/accesspackage.md).  Пользователь, выполняющий запрос, должен уже существовать в каталоге.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [акцесспаккажеассигнментрекуест](../resources/accesspackageassignmentrequest.md) в тексте отклика.  

Если это `AdminAdd` запрос, затем [акцесспаккажеассигнмент](../resources/accesspackageassignment.md) и, при необходимости, также создаются [акцесспаккажесубжект](../resources/accesspackagesubject.md) . Вы можете указать их, используя параметры запроса при [выводе акцесспаккажеассигнментс](accesspackageassignment-list.md).

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса для прямого назначения, в котором администратор запрашивает создание назначения для пользователя. Так как [акцесспаккажесубжект](../resources/accesspackagesubject.md) может еще не существовать, значение **TARGETID** — это идентификатор объекта, которому назначен пользователь, значение **акцесспаккажеид** — это необходимый пакет доступа для этого пользователя, а значение **ассигнментполициид** — это прямая политика назначения в этом пакете доступа.
 

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "AdminAdd",
  "accessPackageAssignment":{
     "targetId":"46184453-e63b-4f20-86c2-c557ed5d5df9",
     "assignmentPolicyId":"2264bf65-76ba-417b-a27d-54d291f0cbc8",
     "accessPackageId":"a914b616-e04e-476b-aa37-91038f0b165b"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackageassignmentrequest-from-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{

  "id": "7e382d02-4454-436b-b700-59c7dd77f466",
  "requestType": "AdminAdd",
  "requestState": "Submitted",
  "requestStatus": "Accepted",
  "isValidationOnly": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


