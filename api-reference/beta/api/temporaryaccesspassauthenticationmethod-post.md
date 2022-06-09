---
title: Создание temporaryAccessPassAuthenticationMethod
description: Создайте новый временный объектAccessPassAuthenticationMethod.
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 43d4b5df97653498c4c3630cb95ca5abb48a9a60
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971576"
---
# <a name="create-temporaryaccesspassauthenticationmethod"></a>Создание temporaryAccessPassAuthenticationMethod
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [временный объектAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) для пользователя. У пользователя может быть только один временный проход доступа. Секретный код можно использовать между временем начала и окончания временного прохода доступа. Если пользователю требуется новый временный секретный код:
* Хотя текущий временный секретный код действителен, администратору необходимо удалить существующий временный секретный код и создать новый проход для пользователя. Удаление допустимого временного прохода доступа отменит сеансы пользователя. 
* По истечении срока действия временного прохода доступа новый временный проход доступа переопределяет текущий временный проход доступа и не отменяет сеансы пользователя.


## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:---------------------------------------|:-------------------------|
| Делегированные (рабочая или учебная учетная запись)     | UserAuthenticationMethod.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | UserAuthenticationMethod.ReadWrite.All |

В делегированных сценариях, когда администратор действует с другим пользователем, администратору требуется одна из следующих ролей [Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):
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

|Свойство|Тип|Описание|Обязательный| 
|:---|:---|:---|:---|
|startDateTime|DateTimeOffset|Дата и время, когда temporaryAccessPass становится доступным для использования, если временный секретный код не задается, доступен для использования во время создания.| Нет|
|lifetimeInMinutes|Int32|Время существования temporaryAccessPass в минутах, начиная со времени создания или при значении startDateTime, если оно задано. Минимум 10, максимум 43200 (эквивалентно 30 дням).| Нет|
|isUsableOnce|Boolean|Определяет, ограничен ли проход одним использованием. Если значение равно True, то проход можно использовать один раз, если значение равно False, то этот проход можно использовать несколько раз в течение временного жизненного циклаAccessPass. Многопользовательский временный секретный код (isUsableOnce = false) можно создать и использовать для входа только в том случае, если это разрешено политикой метода проверки подлинности временного прохода доступа.|  Нет|



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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-temporaryaccesspassauthenticationmethod-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-temporaryaccesspassauthenticationmethod-from--powershell-snippets.md)]
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
