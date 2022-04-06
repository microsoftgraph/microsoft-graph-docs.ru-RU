---
title: Создание oAuth2PermissionGrant (делегированная субсидия на разрешение)
description: Создайте объект oAuth2PermissionGrant, представляющий делегированную выдачу разрешений.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 6cf8bcb16fe61fa6360adc3aa71b6157445fa644
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2022
ms.locfileid: "63668502"
---
# <a name="create-oauth2permissiongrant-a-delegated-permission-grant"></a>Создание oAuth2PermissionGrant (делегированная субсидия на разрешение)

Пространство имен: microsoft.graph


Создайте делегированную выдачу разрешений, представленную объектом [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) .

Делегированная выдача разрешений разрешает директору клиентской службы (представляющим клиентскую заявку) получать доступ к директору службы ресурсов (представляющим API) от имени подписанного пользователя, для уровня доступа, ограниченного делегированных разрешений, которые были предоставлены.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All    |
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

В теле запроса поставляем представление JSON объекта [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) .

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика 200-й серии и новый [объект oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в тексте отклика. В следующей таблице показаны свойства, необходимые при создании [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| clientId | String | **ID директора** клиентской службы для приложения, которому разрешено действовать от имени пользователя, входишего в него, при доступе к API.[](../resources/serviceprincipal.md) Обязательный.  |
| consentType | String | Указывает, предоставляется ли авторизация клиентского приложения для выдают себя за всех пользователей или только определенного пользователя. *AllPrincipals* указывает авторизацию, чтобы выдать себя за всех пользователей. *Principal* указывает авторизацию, чтобы выдать себя за конкретного пользователя. Согласие от имени всех пользователей может быть предоставлено администратором. В некоторых случаях для некоторых делегированных разрешений пользователям, не относя правительственным администраторам, может быть разрешено согласие от имени самих себя. Обязательный.  |
| principalId | String | **ID пользователя**[,](../resources/user.md) от имени которого клиент уполномочен получать доступ к ресурсу, если **consentType** является *основным*. Если **consentType** *— это AllPrincipals* , это значение является null. Обязательно, когда **consentType** является *основным*. |
| resourceId | String | **ID главного** ресурса [службы,](../resources/serviceprincipal.md) к которому разрешен доступ. При этом определяется API, который клиент уполномочен пытаться вызвать от имени подписанного пользователя. |
| scope | String | Разделенный пробелом список значений утверждений для делегирования разрешений, которые должны быть включены в маркеры доступа для приложения-ресурса (API). Например, `openid User.Read GroupMember.Read.All`. Каждое значение утверждения должно соответствовать значению одного из делегированных разрешений, определенных API, перечисленных в **свойстве oauth2PermissionScopes** директора [службы ресурсов](../resources/serviceprincipal.md). |

## <a name="example"></a>Пример

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_oAuth2PermissionGrant"
}-->

```http
POST https://graph.microsoft.com/v1.0/oauth2PermissionGrants
Content-Type: application/json

{
    "clientId": "ef969797-201d-4f6b-960c-e9ed5f31dab5",
    "consentType": "AllPrincipals",
    "resourceId": "943603e4-e787-4fe9-93d1-e30f749aae39",
    "scope": "DelegatedPermissionGrant.ReadWrite.All"
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/post-oauth2permissiongrant-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/post-oauth2permissiongrant-powershell-snippets.md)]
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#oauth2PermissionGrants/$entity",
    "clientId": "ef969797-201d-4f6b-960c-e9ed5f31dab5",
    "consentType": "AllPrincipals",
    "id": "l5eW7x0ga0-WDOntXzHateQDNpSH5-lPk9HjD3Sarjk",
    "principalId": null,
    "resourceId": "943603e4-e787-4fe9-93d1-e30f749aae39",
    "scope": "DelegatedPermissionGrant.ReadWrite.All"
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

