---
title: Обновление phoneAuthenticationMethod
description: Обновление номера телефона, связанного с объектом phoneAuthenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5230ca00a63f3543b95ef4f2a1dc7242c5460a1b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055409"
---
# <a name="update-phoneauthenticationmethod"></a>Обновление phoneAuthenticationMethod

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление номера телефона, связанного с [методом проверки подлинности телефона.](../resources/phoneauthenticationmethod.md)

Вы не можете изменить тип телефона. Чтобы изменить тип телефона, добавьте новый номер нужного типа и удалите объект с помощью исходного типа.

Если политика позволяет пользователю использовать SMS для входа и изменить номер, система попытается зарегистрировать номер для использования `mobile` в этой системе.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="permissions-acting-on-self"></a>Разрешения, действующие на себя

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:---------------------------------------|:-------------------------|
| Делегированные (рабочая или учебная учетная запись)     | UserAuthenticationMethod.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

### <a name="permissions-acting-on-other-users"></a>Разрешения, действующие на других пользователей

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:---------------------------------------|:-------------------------|
| Делегированные (рабочая или учебная учетная запись)     | UserAuthenticationMethod.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение                            | UserAuthenticationMethod.ReadWrite.All |

Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)
* Глобальный администратор
* Привилегированный администратор проверки подлинности
* Администратор проверки подлинности

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PUT /me/authentication/phoneMethods/{id}
PUT /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```
Значение, `id` соответствующее обновлению phoneType, является одним из следующих:
+ `b6332ec1-7057-4abe-9331-3d72feddfe41` обновление `alternateMobile` **phoneType**.
+ `e37fc753-ff3b-4958-9484-eaa9425c82bc` обновление `office` **phoneType**.
+ `3179e48a-750b-4051-897c-87b9720928f7` обновление `mobile` **phoneType**.

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Описание|
|:-----------|:-----------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Существующие свойства, не включенные в тело запроса, будут пересчитаны в зависимости от изменений в других значениях свойств.

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|phoneNumber|String|Номер телефона для текста или вызова для проверки подлинности. Телефон номера используют формат "+ \<country code\> \<number\> \<extension\> x", с необязательным расширением. Например, допустимы +1 5555551234 или +1 5555551234x1233. При создании и обновлении номера отклоняется, если они не соответствуют требуемой форме.|
|phoneType|String| Возможные значения: `mobile`, `alternateMobile` или `office`.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_phoneauthenticationmethod"
}-->

```http
PUT https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
Content-type: application/json

{
  "phoneNumber": "+1 2065555554",
  "phoneType": "mobile",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "phoneNumber": "+1 2065555554",
  "phoneType": "mobile",
  "smsSignInState": "ready",
  "id": "3179e48a-750b-4051-897c-87b9720928f7"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update phoneauthenticationmethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
