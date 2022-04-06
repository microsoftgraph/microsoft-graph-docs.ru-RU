---
title: Обновление approvalStage
description: Применить утверждение или отказ в принятии решения по объекту approvalStage.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8a3ec53fcd67716de873187c7a34e060cdebc6f4
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516065"
---
# <a name="update-approvalstage"></a>Обновление approvalStage

Пространство имен: microsoft.graph

В [управлении правами Azure AD](../resources/entitlementmanagement-overview.md) утвердите или откажье [объект approvalStage](../resources/approvalstage.md) в [утверждении](../resources/approval.md).

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
PATCH /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{accessPackageAssignmentRequestId}/stages/{approvalStageId}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса

В следующей таблице показаны свойства, необходимые для этого метода.

| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
| reviewResult | String | Решение утвержденного. Возможные значения: `Approve`, `Deny`. Обязательный.|
| обоснование | String | Обоснование, связанное с решением утвержденного. |


## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `204 No Content` ответа в тексте ответа. IOf вызываемого не имеет нужных разрешений, `403 Forbidden` метод возвращает код ответа, или если код утверждения не найден, метод возвращает `404 Not found`. Если запрос уже утвержден другим утверждением на том же этапе утверждения, `409 Conflict` метод возвращает код ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_approvalstage"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/stages/d4fa4045-4716-436d-aec5-57b0a713f095

{
 "reviewResult":"Approve",
 "justification":"OK"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-approvalstage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-approvalstage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-approvalstage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-approvalstage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/patch-approvalstage-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patch approvalStage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
