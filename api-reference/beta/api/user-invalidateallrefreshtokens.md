---
title: 'Пользователь: служебное invalidateallrefreshtokens'
description: Делает недействительными все маркеры обновления пользователя, выданные приложениям (а также файлам cookie сеанса в браузере пользователя), путем сброса свойства пользователя **refreshtokensvalidfromdatetime и указывая** к текущей дате и времени. Как правило, эта операция выполняется (пользователем или администратором), если пользователь имеет утерянное или украденное устройство.  Эта операция запрещает доступ к данным в Организации, доступ к которым осуществляется через приложения на устройстве, без необходимости первого входа пользователя в систему. В действительности эта операция приведет к принудительному входу пользователя в систему для всех приложений, для которых они ранее были отправлены, независимо от устройства.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c8f5f38b3c3ee979f0b411ca01c7629e16fbe958
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270310"
---
# <a name="user-invalidateallrefreshtokens"></a>Пользователь: служебное invalidateallrefreshtokens

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Делает недействительными все маркеры обновления пользователя, выданные приложениям (а также файлам cookie сеанса в браузере пользователя), путем сброса свойства пользователя **refreshtokensvalidfromdatetime и указывая** к текущей дате и времени. Как правило, эта операция выполняется (пользователем или администратором), если пользователь имеет утерянное или украденное устройство.  Эта операция запрещает доступ к данным в Организации, доступ к которым осуществляется через приложения на устройстве, без необходимости первого входа пользователя в систему. В действительности эта операция приведет к принудительному входу пользователя в систему для всех приложений, для которых они ранее были отправлены, независимо от устройства.

Для разработчиков, если приложение пытается активировать маркер делегированного доступа для этого пользователя с помощью недействительного маркера обновления, приложение получит сообщение об ошибке. В этом случае приложению потребуется получить новый маркер обновления, выполнив запрос к конечной точке авторизации, которая вынуждает пользователя выполнить вход.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

+ Чтобы приложение, вошедшего в систему, не проверяло приложения, на которые они были отправлены: User. ReadWrite, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL
+ Для приложения, позволяющего администратору сделать недействительными приложения, которые пользователь прослал: Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/invalidateAllRefreshTokens
POST /users/{id | userPrincipalName}/invalidateAllRefreshTokens
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Тело запроса
В этой операции нет содержимого запроса.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "user_invalidateallrefreshtokens"
}-->
```http
POST https://graph.microsoft.com/beta/me/invalidateAllRefreshTokens
```

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/user_invalidateallrefreshtokens-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_invalidateallrefreshtokens-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_invalidateallrefreshtokens-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-invalidateallrefreshtokens.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-invalidateallrefreshtokens.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-invalidateallrefreshtokens.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
