---
title: Обновление аусоризатионполици
description: Обновление свойств объекта Аусоризатионполици.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ddb7d869c45fe727a962c280d8c4cdd8c07f2432
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/16/2020
ms.locfileid: "47842913"
---
# <a name="update-authorizationpolicy"></a>Обновление Аусоризатионполици

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [аусоризатионполици](../resources/authorizationpolicy.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Policy. ReadWrite. Authorization|
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Policy. ReadWrite. Authorization|

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Authorization | Bearer {token} |
| Content-Type | application/json |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|  
|displayName|String| Отображаемое имя для этой политики. |  
|description|String| Описание этой политики. |  
|гуестусерролеид|Guid| Представляет templateId роли для роли, которая должна быть выделена пользователю "гость". Обратитесь к [списку унифиедроледефинитионс](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) , чтобы найти список доступных шаблонов ролей. Только поддерживаемые роли: User (a0b1b346-4d3e-4e8b-98f8-753987be4970), гость (10dae51f-b6af-4016-8d66-8c2a99b929b3) и пользователь с ограниченным гостями (2af84b1e-32c8-42b7-82bc-daa82404023b). | 
|енабледпревиевфеатурес|Коллекция (String)| Список компонентов, включенных для закрытой предварительной версии в клиенте. | 
|блоккмсолповершелл|Boolean| Чтобы отключить использование MSOL PowerShell, задайте для этого свойства значение `true` . Параметр `true` также отключит доступ пользователей к устаревшей конечной точке службы, используемой MSOL PowerShell. Это не повлияет на Azure AD Connect или Microsoft Graph. | 
|defaultUserRolePermissions|[defaultUserRolePermissions](../resources/defaultUserRolePermissions.md)| Задает определенные настраиваемые разрешения для роли пользователя по умолчанию. | 
|allowedToUseSSPR|Boolean| Указывает, можно ли использовать функцию самостоятельного сброса пароля для пользователей клиента. | 
|allowedToSignUpEmailBasedSubscriptions|Boolean| Указывает, могут ли пользователи регистрироваться на почтовые подписки. | 
|allowEmailVerifiedUsersToJoinOrganization|Boolean| Указывает, может ли пользователь присоединиться к клиенту по проверке электронной почты. | 

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a>Пример 1: обновление или Настройка уровня доступа гостей для клиента

#### <a name="request"></a>Запрос

Ниже приведен пример запроса. В этом примере уровень гостевого доступа изменяется на "ограниченный гостевой пользователь".

<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_guestUserLevel"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
  "guestUserRole": "2af84b1e-32c8-42b7-82bc-daa82404023b"
}

```
#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content

```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a>Пример 2: включение новой функции для предварительного просмотра в клиенте

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_preview"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
  "enabledPreviewFeatures": ["assignGroupsToRoles"]
}

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-preview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-preview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-preview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```


### <a name="example-3-block-msol-powershell-in-tenant"></a>Пример 3: Блокировка MSOL PowerShell в клиенте

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_blockMSOLPowerShell"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
  "blockMsolPowerShell": true
}

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-blockmsolpowershell-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-blockmsolpowershell-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-blockmsolpowershell-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
### <a name="example-4-disable-default-user-roles-permission-to-create-applications"></a>Пример 4: отключение разрешения роли пользователя по умолчанию для создания приложений

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_applications"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
    "defaultUserRolePermissions":
    {
      "allowedToCreateApps": false
    }
}

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-applications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-applications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-applications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-5-enable-default-user-role-to-use-self-serve-password-reset-feature"></a>Пример 5: Включение роли пользователя по умолчанию для использования функции самостоятельного сброса пароля

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authZPolicy_SSPR"
}-->

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy

{
    "allowedToUseSSPR": true
}

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authzpolicy-sspr-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authzpolicy-sspr-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authzpolicy-sspr-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
