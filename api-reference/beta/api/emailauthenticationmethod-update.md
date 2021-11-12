---
title: Обновление emailAuthenticationMethod
description: Обновление свойств объекта emailAuthenticationMethod.
author: mmcla
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 845da699f158ac954e2090b23f6c193a903a4adb
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60925245"
---
# <a name="update-emailauthenticationmethod"></a>Обновление emailAuthenticationMethod
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление электронного адреса пользователя, связанного с объектом [метода проверки подлинности электронной](../resources/emailauthenticationmethod.md) почты.

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
| Для приложений                            | UserAuthenticationMethod.ReadWrite.All |

Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)

* Глобальный администратор
* Привилегированный администратор проверки подлинности
* Администратор проверки подлинности

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем JSON-представление объекта [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) с обновленным адресом электронной почты.

В следующей таблице показаны свойства, необходимые при обновлении [электронной почтыAuthenticationMethod.](../resources/emailauthenticationmethod.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|emailAddress|String|Обновленный адрес электронной почты|



## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_emailauthenticationmethod"
}
-->
``` http
PUT https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
Content-Type: application/json

{
  "emailAddress": "kim@contoso.com"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик

Ниже приведен пример ответа.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethod"
} -->

``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
  "emailAddress": "kim@contoso.com"
}
```
