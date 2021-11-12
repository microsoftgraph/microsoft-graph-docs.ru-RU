---
title: Создание temporaryAccessPassAuthenticationMethod
description: Создание нового объекта temporaryAccessPassAuthenticationMethod.
author: inbarckMS
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 55f75409c57e7b676dcf93456cab2391a51cd88b
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60941962"
---
# <a name="create-temporaryaccesspassauthenticationmethod"></a>Создание temporaryAccessPassAuthenticationMethod
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) для пользователя. У пользователя может быть только один временный пропуск доступа. Пароль можно использовать между началом и конечным временем временного пропуска доступа. Если пользователю требуется новый временный пропуск доступа:
* Хотя текущий пропуск временного доступа действителен, администратору необходимо удалить существующий временный пропуск доступа и создать новый пропуск для пользователя. Удаление допустимой временной пропускной записи отзовет сеансы пользователя. 
* После истечения срока действия временного пропуска доступа новый временный пропуск переопределит текущий временный пропуск доступа и не отменит сеансы пользователя.


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

Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)
* Глобальный администратор
* Привилегированный администратор проверки подлинности
* Администратор проверки подлинности

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
В теле запроса поставляем представление JSON объекта [temporaryAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)

В следующей таблице описываются необязательные свойства, которые можно использовать при создании [временногоAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)

|Свойство|Тип|Описание|Обязательный| 
|:---|:---|:---|:---|
|startDateTime|DateTimeOffset|Дата и время, когда временныйAccessPass станет доступным для использования, если не задать временный пропуск доступа, можно использовать во время создания.| Нет|
|lifetimeInMinutes|Int32|Срок службы temporaryAccessPass в минутах, начиная с момента создания или при наборе startDateTime. Минимум 10, максимум 43200 (эквивалент 30 дней).| Нет|
|isUsableOnce|Логический|Определяет, ограничен ли пропуск одно время использования. Если true — пропуск можно использовать один раз, если false — пропуск можно использовать несколько раз в течение временного времени службыAccessPass. Многоцелевой временный пропуск доступа (isUsableOnce = false) может быть создан и использован для регистрации, если это разрешено политикой метода проверки подлинности временного доступа.|  Нет|



## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и временный `201 Created` [объектAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_temporaryaccesspassauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "startDateTime": "2021-01-26T00:00:00.000Z",
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

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-temporaryaccesspassauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-temporaryaccesspassauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
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
    "id": "81757535-e21e-4330-a338-33b8038ff12b",
    "temporaryAccessPass": "nc+&G=xwDKCz",
    "createdDateTime": "2021-01-25T23:53:35.5026721Z",
    "startDateTime": "2021-01-26T00:00:00Z",
    "lifetimeInMinutes": 60,
    "isUsableOnce": false,
    "isUsable": false,
    "methodUsabilityReason": "NotYetValid"

}
```
