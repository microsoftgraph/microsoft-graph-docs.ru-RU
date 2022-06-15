---
title: Создание temporaryAccessPassMethod
description: Создайте новый временный объектAccessPassAuthenticationMethod для пользователя.
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 2d0dbd6ecb3bf9e2aa260496d096ee6278b44539
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093348"
---
# <a name="create-temporaryaccesspassmethod"></a>Создание temporaryAccessPassMethod
Пространство имен: microsoft.graph

Создайте новый [временный объектAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) для пользователя. У пользователя может быть только один временный секретный код, который можно использовать в течение указанного времени существования. Если пользователю требуется новый временный секретный код, пока текущий временный секретный код действителен, администратор может создать новый временный секретный код для пользователя, предыдущий временный проход доступа будет удален и создан новый временный секретный код.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

### <a name="permissions-acting-on-other-users"></a>Разрешения, действующие на других пользователей

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:---------------------------------------|:-------------------------|
| Делегированные (рабочая или учебная учетная запись)     | UserAuthenticationMethod.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение                            | UserAuthenticationMethod.ReadWrite.All |

В делегированных сценариях, когда администратор действует с другим пользователем, администратору требуется одна из следующих Azure AD [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):
* глобальный администратор;
* привилегированный администратор проверки подлинности;
* администратор проверки подлинности.

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) в формате JSON.

В следующей таблице описаны необязательные свойства, которые можно использовать при создании [временного объектаAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|isUsableOnce|Boolean|Необязательное свойство. Определяет, ограничен ли проход однофакторным использованием. Если `true`этот проход можно использовать один раз; если `false`этот проход можно использовать несколько раз в течение времени **существования ПараметрInMinutes** . Многопользовательский временный секретный код (`isUsableOnce = false`) можно создать и использовать для входа только в том случае, если это разрешено политикой метода проверки подлинности временного  [прохода доступа](../resources/temporaryaccesspassauthenticationmethodconfiguration.md).|
|lifetimeInMinutes|Int32|Необязательный. Время существования temporaryAccessPass в минутах, начиная со времени создания или при значении startDateTime, если оно задано. Должно быть от 10 до 43200 (эквивалентно 30 дням). Если этот параметр не указан, применяется параметр **defaultLifetimeInMinutes** в политике метода проверки подлинности [временного](../resources/temporaryaccesspassauthenticationmethodconfiguration.md) прохода доступа. |
|startDateTime|DateTimeOffset|Необязательно. Дата и время, когда temporaryAccessPass становится доступным для использования. Если этот параметр не указан, временный секретный код доступен для использования сразу после его создания.| 

## <a name="response"></a>Отклик

В случае успешного выполнения `201 Created` этот метод возвращает код отклика и временный [объектAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_temporaryaccesspassauthenticationmethod_from_"
}
-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/users/071cc716-8147-4397-a5ba-b2105951cc0b/authentication/temporaryAccessPassMethods
Content-Type: application/json

{
    "startDateTime": "2022-06-05T00:00:00.000Z",
    "lifetimeInMinutes": 60,
    "isUsableOnce": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-temporaryaccesspassauthenticationmethod-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-temporaryaccesspassauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-temporaryaccesspassauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-temporaryaccesspassauthenticationmethod-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
    "id": "6f1967b7-15e8-4935-ac26-d50770ed07a7",
    "temporaryAccessPass": "+drkzqAD",
    "createdDateTime": "2022-06-02T16:21:09.765173Z",
    "startDateTime": "2022-06-05T00:00:00Z",
    "lifetimeInMinutes": 60,
    "isUsableOnce": false,
    "isUsable": false,
    "methodUsabilityReason": "NotYetValid"
}
```
