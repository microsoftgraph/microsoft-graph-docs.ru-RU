---
title: Обновление b2cAuthenticationMethodsPolicy
description: Обновление свойств объекта b2cAuthenticationMethodsPolicy.
localization_priority: Priority
author: namkedia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aed20c26bab07cb6778b80d10e3becf33e998409
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961282"
---
# <a name="update-b2cauthenticationmethodspolicy"></a>Обновление b2cAuthenticationMethodsPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения|
|:---------------------------------------|:---------------|
| Делегированное (рабочая или учебная учетная запись)     | Policy.ReadWrite.AuthenticationMethod|
| Делегированное (личная учетная запись Майкрософт) | Policy.ReadWrite.AuthenticationMethod|
| Для приложений                            | Policy.ReadWrite.AuthenticationMethod|

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/b2cAuthenticationMethodsPolicy
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте описание объекта [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md) в формате JSON.

В таблице ниже показаны свойства, требуемые при обновлении [b2cAuthenticationMethodsPolicy](../resources/b2cauthenticationmethodspolicy.md).

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|isEmailPasswordAuthenticationEnabled|Логическое|Администратор клиента может настраивать локальные учетные записи, используя электронную почту, если включен метод проверки подлинности электронной почты и пароля.|
|isUserNameAuthenticationEnabled|Логический|Администратор клиента может настраивать локальные учетные записи, используя имя пользователя, если включен метод проверки подлинности электронной почты и пароля.|

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_b2cauthenticationmethodspolicy"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/policies/b2cAuthenticationMethodsPolicy

{
    "isEmailPasswordAuthenticationEnabled": false,
    "isUserNameAuthenticationEnabled": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-b2cauthenticationmethodspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-b2cauthenticationmethodspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-b2cauthenticationmethodspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-b2cauthenticationmethodspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cauthenticationmethodspolicy"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update b2cauthenticationmethodspolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
