---
title: 'пользователь: validatePassword'
description: Проверьте пароль пользователя в отношении политики проверки паролей организации и сообщайте, является ли пароль допустимым.
author: yyuank
ms.localizationpriority: medium
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 499aa0aebc2df0e27a8469070d66628897b585f8
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340930"
---
# <a name="user-validatepassword"></a>пользователь: validatePassword
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Проверьте пароль пользователя в отношении политики проверки паролей организации и сообщайте, является ли пароль допустимым. Используйте это действие, чтобы обеспечить обратную связь в режиме реального времени о силе пароля, пока пользователь типа их пароль.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)| User.ReadWrite, User.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается. |
|Для приложений| Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/validatePassword
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тело запроса добавьте параметры в формате JSON.

В следующей таблице показаны параметры, необходимые для этого действия.

|Параметр|Тип|Описание|
|:---|:---|:---|
|password|Строка| Пароль, который должен быть проверен этим действием.|

## <a name="response"></a>Отклик

В случае успеха это действие возвращает код `200 OK` отклика и [объект passwordValidationInformation](../resources/passwordvalidationinformation.md) в тексте ответа.

## <a name="examples"></a>Примеры 

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_validatepassword"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/validatePassword
Content-Type: application/json

{
    "password": "1234567890"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-validatepassword-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-validatepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-validatepassword-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-validatepassword-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-validatepassword-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/user-validatepassword-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordValidationInformation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "isValid": false,
    "validationResults": [
        {
            "ruleName": "password_not_meet_complexity",
            "validationPassed": false,
            "message": "Password does not meet complexity requirements."
        }
    ]
}
```

