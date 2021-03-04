---
title: Создание emailAuthenticationMethod
description: Создание нового объекта emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b9ec2d40253faa72fd1f8d354de2649c4487e47e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436330"
---
# <a name="create-emailauthenticationmethod"></a>Создание emailAuthenticationMethod
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Установите объект [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) пользователя. Проверка подлинности электронной почты — это метод сброса пароля самообслуживления. У пользователя может быть только один метод проверки подлинности электронной почты.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения, действующие на себя (от наименее до самых привилегированных)|Разрешения, действующие на других (от наименее привилегированных)|
|:---|:---|:--|
| Делегированные (рабочая или учебная учетная запись)     | UserAuthenticationMethod.ReadWrite | UserAuthenticationMethod.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. | Не поддерживается. |
| Приложение                            | Неприменимо. | UserAuthenticationMethod.ReadWrite.All |

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
POST /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса укажи JSON-представление объекта [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) с нужным адресом электронной почты.

В следующей таблице показаны свойства, необходимые при создании [электронной почтыAuthenticationMethod.](../resources/emailauthenticationmethod.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|emailAddress|String|Адрес электронной почты|



## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и новый объект `201 Created` [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_emailauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods
Content-Type: application/json

{
  "emailAddress": "kim@contoso.com"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-emailauthenticationmethod-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-emailauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
Ниже приведен пример отклика.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
  "emailAddress": "kim@contoso.com"
}
```
