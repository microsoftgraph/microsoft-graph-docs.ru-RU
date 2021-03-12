---
title: 'пользователь: revokeSignInSessions'
description: Недействительными признаны все маркеры обновления пользователя, выданные приложениям (а также cookie-файлы сеансов в браузере пользователя), сбросив свойство **signInSessionsValidFromDateTime** в текущее время даты.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: ed8cbcf1e0b04bc93af06b699f37fe0f693280f5
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721385"
---
# <a name="user-revokesigninsessions"></a>пользователь: revokeSignInSessions

Пространство имен: microsoft.graph

Недействительными признаны все маркеры обновления, выданные приложениям для пользователя (а также cookie-файлы сеансов в браузере пользователя), сбросив свойство **signInSessionsValidFromDateTime** в текущее время даты. Обычно эта операция выполняется (пользователем или администратором), если у пользователя потеряно или украдено устройство. Эта операция предотвращает доступ к данным организации с помощью приложений на устройстве, требуя от пользователя снова войти во все приложения, с которыми они ранее согласились, независимо от устройства.

>Если приложение пытается выкупить делегированный маркер доступа для этого пользователя с помощью недействительных маркеров обновления, приложение получит ошибку. Если это произойдет, приложению потребуется приобрести новый маркер обновления, сделав запрос в конечную точку авторизации, что заставит пользователя войти.

>[!NOTE]
>После вызова **revokeSignInSessions** может возникнуть небольшая задержка в несколько минут до отзыва маркеров.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение                            | User.ReadWrite.All, Directory.ReadWrite.All,|

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
Эта операция не имеет контента запроса.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

>[!NOTE]
>У этого API есть [известная проблема](/graph/known-issues#revoke-sign-in-sessions-returns-wrong-HTTP-code). Он возвращает другой код ответа HTTP.

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

