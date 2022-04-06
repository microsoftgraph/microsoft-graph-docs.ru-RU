---
title: 'passwordAuthenticationMethod: resetPassword'
description: Сброс пароля пользователя
ms.localizationpriority: medium
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3e07320950184a89c9d8000145b75af978a4e1e1
ms.sourcegitcommit: dab085b74666e190974a35e6a124d3ff1645fa25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/05/2022
ms.locfileid: "64646588"
---
# <a name="passwordauthenticationmethod-resetpassword"></a>passwordAuthenticationMethod: resetPassword

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Инициировать сброс пароля, связанного с объектом метода проверки [подлинности](../resources/passwordauthenticationmethod.md) паролей. Это может быть сделано только администратором с соответствующими разрешениями и не может выполняться на собственной учетной записи пользователя.

Этот поток записывает новый пароль для Azure Active Directory и подталкивает его к локальная служба Active Directory при настройке с помощью записи пароля. Администратор может либо предоставить новый пароль, либо создать его в системе. Пользователю предложено изменить пароль при следующем входе.

Этот сброс является длительной операцией и возвращает заглавную ссылку Location со ссылкой, по которой вызываемая может периодически проверять состояние операции сброса.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

> [!IMPORTANT]
> Операция не может выполняться на собственной учетной записи пользователя. Выполнить эту операцию может только администратор с соответствующими разрешениями.

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:---------------------------------------|:-------------------------|
| Делегированные (рабочая или учебная учетная запись)     | UserAuthenticationMethod.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна из следующих ролей [Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):

* глобальный администратор;
* привилегированный администратор проверки подлинности;
* администратор проверки подлинности.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/authentication/passwordMethods/{id}/resetPassword
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {token}. Обязательный. |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип        | Описание |
|:-------------|:------------|:------------|
|newPassword|String|Новый пароль. Требуется для клиентов с гибридными сценариями паролей. Если не будет пропущен пароль только для облака, система возвращает созданный системой пароль. Это строка единого кода без другого кодирования. Он проверяется в отношении запрещенной системы паролей клиента перед принятием и должен соответствовать требованиям облачного и/или локального пароля клиента.|

## <a name="response"></a>Отклик

В случае успешной работы `202 Accepted` этот метод возвращает код ответа и заглавную кнопку Location с URL-адресом для проверки состояния операции сброса.

Если вызываемый не представил пароль, созданный Корпорацией Майкрософт пароль предоставляется в объекте JSON в теле ответа.

### <a name="response-headers"></a>Заголовки откликов

| Имя        | Описание     |
|:------------|:----------------|
|Location     | URL-адрес для вызова, чтобы проверить состояние операции. Обязательный.|
|Retry-after  | Длительность в секундах. Необязательный параметр.|

## <a name="examples"></a>Примеры

### <a name="example-1-user-submitted-password"></a>Пример 1. Пароль, отправленный пользователем

В следующем примере показано, как вызвать этот API при отправке пароля вызываемой.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_adminprovided"
}-->

```http
POST https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword
Content-type: application/json

{
    "newPassword": "Cuyo5459"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/passwordauthenticationmethod-resetpassword-adminprovided-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/passwordauthenticationmethod-resetpassword-adminprovided-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/passwordauthenticationmethod-resetpassword-adminprovided-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/passwordauthenticationmethod-resetpassword-adminprovided-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
} -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json
Location: https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0/authentication/operations/88e7560c-9ebf-435c-8089-c3998ac1ec51?aadgdc=DUB02P&aadgsu=ssprprod-a

{}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod: resetPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

### <a name="example-2-system-generated-password"></a>Пример 2. Созданный системой пароль

В следующем примере показано, как вызывать этот API, если вызываемая не представляет пароль.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "passwordauthenticationmethod_resetpassword_systemgenerated"
}-->

```http
POST https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0/authentication/passwordMethods/28c10230-6103-485e-b985-444c60001490/resetPassword
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/passwordauthenticationmethod-resetpassword-systemgenerated-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/passwordauthenticationmethod-resetpassword-systemgenerated-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/passwordauthenticationmethod-resetpassword-systemgenerated-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/passwordauthenticationmethod-resetpassword-systemgenerated-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
} -->

```http
HTTP/1.1 202 ACCEPTED
Location: https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0/authentication/operations/77bafe36-3ac0-4f89-96e4-a4a5a48da851?aadgdc=DUB02P&aadgsu=ssprprod-a
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.passwordResetResponse",
    "newPassword": "Cuyo5459"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod: resetPassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
