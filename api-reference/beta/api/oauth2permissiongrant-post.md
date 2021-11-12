---
title: Создание oAuth2PermissionGrant (делегированная субсидия на разрешение)
description: Создайте объект oAuth2PermissionGrant, представляющий делегированную выдачу разрешений.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 7132a4825ae2747b28789e88ad1e13fdb9429afc
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890150"
---
# <a name="create-oauth2permissiongrant-a-delegated-permission-grant"></a>Создание oAuth2PermissionGrant (делегированная субсидия на разрешение)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте делегированную выдачу разрешений, представленную [объектом oAuth2PermissionGrant.](../resources/oauth2permissiongrant.md)

Делегированная выдача разрешений разрешает директору клиентской службы (представляющим клиентскую заявку) получать доступ к директору службы ресурсов (представляющим API) от имени подписанного пользователя, для уровня доступа, ограниченного делегированных разрешений, которые были предоставлены.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /oauth2PermissionGrants
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание |
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [oAuth2PermissionGrant.](../resources/oauth2permissiongrant.md)

В следующей таблице показаны свойства, необходимые при создании [oAuth2PermissionGrant.](../resources/oauth2permissiongrant.md)

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| clientId | String | ID **директора** клиентской службы для приложения, которому разрешено действовать от имени пользователя, входишего в него, при доступе к API. [](../resources/serviceprincipal.md) Обязательный.  |
| consentType | String | Указывает, предоставляется ли авторизация клиентского приложения для выдают себя за всех пользователей или только определенного пользователя. *AllPrincipals* указывает авторизацию, чтобы выдать себя за всех пользователей. *Principal* указывает авторизацию, чтобы выдать себя за конкретного пользователя. Согласие от имени всех пользователей может быть предоставлено администратором. В некоторых случаях для некоторых делегированных разрешений пользователям, не относя правительственным администраторам, может быть разрешено согласие от имени самих себя. Обязательный.  |
| principalId | Строка | ID **пользователя,** от имени которого клиент уполномочен получать доступ к ресурсу, если **consentType** является [](../resources/user.md) *основным.* Если **consentType** *— это AllPrincipals,* это значение является null. Обязательно, когда **consentType** является *основным*. |
| resourceId | String | ID **главного** ресурса [службы,](../resources/serviceprincipal.md) к которому разрешен доступ. При этом определяется API, который клиент уполномочен пытаться вызвать от имени подписанного пользователя. |
| scope | String | Разделенный пробелом список значений утверждений для делегирования разрешений, которые должны быть включены в маркеры доступа для приложения-ресурса (API). Например, `openid User.Read GroupMember.Read.All`. Каждое значение утверждения  должно совпадать с полем значения одного из делегированных разрешений, определенных API, перечисленным в свойстве **publishedPermissionScopes** директора [службы ресурсов.](../resources/serviceprincipal.md) |
| startTime | DateTimeOffset | В настоящее время значение времени начала игнорируется, но требуется значение. Обязательный. |
| expiryTime | DateTimeOffset | В настоящее время значение конца времени игнорируется, но требуется значение. Обязательный. |

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика 200-й серии и новый [объект oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_oAuth2PermissionGrant"
}-->

```http
POST https://graph.microsoft.com/beta/oauth2PermissionGrants
Content-Type: application/json

{
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "scope": "scope-value",
  "startTime": "2016-10-19T10:37:00Z",
  "expiryTime": "2016-10-19T10:37:00Z"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "id-value",
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "scope": "scope-value",
  "startTime": "2016-10-19T10:37:00Z",
  "expiryTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


