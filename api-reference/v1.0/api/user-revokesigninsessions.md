---
title: 'Пользователь: Ревокесигнинсессионс'
description: Делает недействительным все маркеры обновления пользователя, выданные приложениям (а также файлам cookie сеанса в браузере пользователя), путем сброса свойства пользователя **сигнинсессионсвалидфромдатетиме** к текущей дате и времени.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d2c5104723e3dbe4a775f7905e04def52fe32283
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508935"
---
# <a name="user-revokesigninsessions"></a>Пользователь: Ревокесигнинсессионс

Пространство имен: microsoft.graph

Делает недействительными все маркеры обновления, выданные приложениям для пользователя (а также файлы cookie сеансов в браузере пользователя), путем сброса свойства пользователя **сигнинсессионсвалидфромдатетиме** к текущей дате и времени. Как правило, эта операция выполняется (пользователем или администратором), если пользователь имеет утерянное или украденное устройство. Эта операция запрещает доступ к данным Организации через приложения на устройстве, требуя от пользователя повторного входа во все приложения, которые ранее были отосланы, независимо от устройства.

>Если приложение пытается активировать маркер делегированного доступа для этого пользователя с помощью недействительного маркера обновления, приложение получит ошибку. В этом случае приложению потребуется получить новый маркер обновления, выполнив запрос к конечной точке авторизации, которая вынуждает пользователя выполнить вход.

>[!NOTE]
>После вызова **ревокесигнинсессионс**может возникнуть небольшая задержка в несколько минут до отзыва маркеров.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | User. ReadWrite, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Directory.ReadWrite.All, Directory.AccessAsUser.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/revokeSignInSessions
POST /users/{id | userPrincipalName}/revokeSignInSessions
```

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса
В этой операции нет содержимого запроса.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

>[!NOTE]
>У этого API есть [известная проблема](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code). Он возвращает другой код HTTP-ответа.

## <a name="example"></a>Пример
В приведенном ниже примере показано, как вызывать этот API.

##### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/revokeSignInSessions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-revokesigninsessionss-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-revokesigninsessionss-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-revokesigninsessionss-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-revokesigninsessionss-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: revokeSignInSessions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
