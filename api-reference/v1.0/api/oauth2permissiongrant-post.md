---
title: Создание oAuth2PermissionGrant (делегированное предоставление разрешений)
description: Создайте объект oAuth2PermissionGrant, представляющий делегированное предоставление разрешений.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: dfbd40b52ecc59ce7dc55aa54e86cb24dd7d0cbf
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060509"
---
# <a name="create-oauth2permissiongrant-a-delegated-permission-grant"></a>Создание oAuth2PermissionGrant (делегированное предоставление разрешений)

Пространство имен: microsoft.graph


Создание делегированного разрешения, представленного [объектом oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) .

Делегированное разрешение разрешает субъекту-службе клиента (представляющее клиентское приложение) доступ к субъекту-службе ресурса (представляющего API) от имени вошедщего пользователя на уровень доступа, ограниченный делегированными разрешениями, которые были предоставлены.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись) | DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All    |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All |

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

В тексте запроса добавьте представление объекта [oAuth2PermissionGrant в формате JSON](../resources/oauth2permissiongrant.md) .

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика серии 200 и новый объект [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) в теле отклика. В следующей таблице показаны свойства, необходимые при создании [объекта oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| clientId | String | Идентификатор **субъекта-службы** клиента для приложения, которому разрешено действовать от имени вошедвшего пользователя при доступе к API.[](../resources/serviceprincipal.md) Обязательный.  |
| consentType | String | Указывает, предоставляется ли клиентское приложение авторизации для олицетворения всех пользователей или только определенного пользователя. *AllPrincipals* указывает авторизацию для олицетворения всех пользователей. *Субъект* указывает авторизацию для олицетворения определенного пользователя. Согласие от имени всех пользователей может предоставить администратор. В некоторых случаях пользователи, не являемые администраторами, могут иметь разрешение на предоставление согласия от имени себя для некоторых делегированных разрешений. Обязательный.  |
| principalId | String | Идентификатор **пользователя,** от имени [](../resources/user.md) которого клиент имеет право на доступ к ресурсу, если **consentType** имеет значение *Principal*. Если **consentType** имеет *значение AllPrincipals* , это значение равно NULL. Требуется, если **consentType является principal***.* |
| resourceId | String | Идентификатор **субъекта-службы** [ресурсов](../resources/serviceprincipal.md) , к которому авторизован доступ. Это определяет API, клиент которого имеет право на попытку вызова от имени вошедвшего пользователя. |
| scope | String | Разделенный пробелами список значений утверждений для делегированных разрешений, которые должны быть включены в маркеры доступа для приложения ресурсов (API). Например, `openid User.Read GroupMember.Read.All`. Каждое значение утверждения должно соответствовать полю значения одного из делегированных разрешений, определенных API, перечисленным в свойстве **oauth2PermissionScopes**  субъекта-службы [ресурсов](../resources/serviceprincipal.md). |

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

