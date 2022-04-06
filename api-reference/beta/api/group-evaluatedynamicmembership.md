---
title: 'группа: оценкаDynamicMembership'
description: Оцените, является ли пользователь или устройство членом динамической группы.
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e02843f0d4305388b40d6c5d3bf1e73980b72c89
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64588906"
---
# <a name="group-evaluatedynamicmembership"></a>группа: оценкаDynamicMembership

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определите, может ли пользователь или устройство являться членом динамической группы. Правило членства возвращается вместе с другими сведениями, которые были использованы в оценке. Эту операцию можно выполнить следующими способами:

- Оцените, является ли пользователь или устройство членом указанной динамической группы.
- Оцените, будет ли пользователь или устройство членом динамической группы на основе ID пользователя или устройства и правила членства.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="evaluate-dynamic-membership-with-member-id-and-group-id"></a>Оценка динамического членства с помощью ID участника и группового ИД

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                                                                          |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Для пользователя: Group.Read.All и User.Read.All, Directory.Read.All<br>Для устройства: Group.Read.All и Device.Read.All, Directory.Read.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                                                                                                       |
| Для приложений                            | Не поддерживается.                                                                                                                       |

### <a name="evaluate-dynamic-membership-with-member-id-and-membership-rule"></a>Оценка динамического членства с помощью ID и правила членства

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)                                                    |
| :------------------------------------- | :--------------------------------------------------------------------------------------------- |
| Делегированные (рабочая или учебная учетная запись)     | Для пользователя: User.Read.All, Directory.Read.All<br>Для устройства: Device.Read.All, Directory.Read.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                                                                                 |
| Для приложений                            | Не поддерживается.                                                                                 |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/evaluateDynamicMembership
POST /groups/evaluateDynamicMembership
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание      |
| :------------ | :--------------- |
| Авторизация | Bearer {token}   |
| Content-Type  | application/json |

## <a name="request-body"></a>Текст запроса

В теле запроса укажи необходимые свойства.

В следующей таблице перечислены свойства, необходимые при оценке членства в группе.

| Параметр      | Тип              | Описание                                                                                                                                                                                                                                                                                                                                                                                                            |
| :------------- | :---------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| memberId       | Коллекция строк | memberId — это объектный id пользователя или устройства, для оценки.                                                                                                                                                                                                                                                                                                                                                       |
| membershipRule | Коллекция строк | Правило, которое используется для оценки членства. Если это свойство не предоставлено, оценивается правило для существующей группы. Если это свойство предоставлено, пользователь или устройство оцениваются для возможного членства в группе с тем же правилом. Дополнительные сведения можно найти в статье [Правила динамического членства в группах для Azure AD](/azure/active-directory/users-groups-roles/groups-dynamic-membership). |

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` ответа и [объект evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) .

## <a name="examples"></a>Примеры

### <a name="example-1-evaluate-if-a-user-or-device-is-a-member-of-an-existing-group"></a>Пример 1. Оценка того, является ли пользователь или устройство членом существующей группы

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership_1"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/evaluateDynamicMembership
Content-type: application/json

{
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33"
}
```

# <a name="c"></a>[C#](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [sample-code](../includes/snippets/go/group-evaluatedynamicmembership-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)

[!INCLUDE [sample-code](../includes/snippets/powershell/group-evaluatedynamicmembership-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")",
  "membershipRuleEvaluationResult": true,
  "membershipRuleEvaluationDetails": {
    "expressionResult": true,
    "expression": "user.displayName -startsWith \"EndTestUser\"",
    "propertyToEvaluate": {
      "propertyName": "displayName",
      "propertyValue": "EndTestUser001"
    }
  }
}

```

### <a name="example-2-evaluate-if-a-user-or-device-would-be-a-member-of-a-group-based-on-a-membership-rule"></a>Пример 2. Оценка того, будет ли пользователь или устройство членом группы на основе правила членства

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership_2"
}-->

```http
POST https://graph.microsoft.com/beta/groups/evaluateDynamicMembership
Content-type: application/json

{
  "memberId": "319b41e8-d9e4-42f8-bdc9-741113f48b33",
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")"
}
```

# <a name="c"></a>[C#](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/group-evaluatedynamicmembership-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/group-evaluatedynamicmembership-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/group-evaluatedynamicmembership-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](../includes/snippets/java/group-evaluatedynamicmembership-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)

[!INCLUDE [sample-code](../includes/snippets/go/group-evaluatedynamicmembership-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "membershipRule": "(user.displayName -startsWith \"EndTestUser\")",
  "membershipRuleEvaluationResult": true,
  "membershipRuleEvaluationDetails": {
    "expressionResult": true,
    "expression": "user.displayName -startsWith \"EndTestUser\"",
    "propertyToEvaluate": {
      "propertyName": "displayName",
      "propertyValue": "EndTestUser001"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "group: evaluateDynamicMembership",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
