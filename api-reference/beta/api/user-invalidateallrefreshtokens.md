---
title: 'пользователь: invalidateAllRefreshTokens'
description: Признает недействительным всех маркеров обновления пользователя, выданный приложений (а также файлы cookie сеанса в браузере пользователя), сброс свойство пользователя **refreshTokensValidFromDateTime** текущая дата и время. Как правило эта операция выполняется (по пользователь или администратор), если у пользователя есть потерянных или украденных устройств.  Эта операция может запретить доступ к любой из организации данных, доступных через приложения на устройстве без уведомления пользователя, сначала необходимо выполнить повторный вход. На самом деле эта операция будет принудительно пользователя выполнить повторный вход для всех приложений, которые они ранее согласие, вне зависимости от устройства.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c006787c0d68ae0c6ecbb331a9ff410f957a6f93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524529"
---
# <a name="user-invalidateallrefreshtokens"></a>пользователь: invalidateAllRefreshTokens

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Признает недействительным всех маркеров обновления пользователя, выданный приложений (а также файлы cookie сеанса в браузере пользователя), сброс свойство пользователя **refreshTokensValidFromDateTime** текущая дата и время. Как правило эта операция выполняется (по пользователь или администратор), если у пользователя есть потерянных или украденных устройств.  Эта операция может запретить доступ к любой из организации данных, доступных через приложения на устройстве без уведомления пользователя, сначала необходимо выполнить повторный вход. На самом деле эта операция будет принудительно пользователя выполнить повторный вход для всех приложений, которые они ранее согласие, вне зависимости от устройства.

Для разработчиков Если приложение пытается использовать маркер делегированные доступа для этого пользователя с помощью маркера недействительным обновления приложения появится сообщение об ошибке. В этом случае приложения необходимо получить новый маркер обновления при выполнении запроса к конечной точке авторизовать, которая отвечает за выполнение принудительной пользователи могут входить в.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

+ Приложение может разрешить подписанных в пользователю недействительными приложений они согласие на: User.ReadWrite, Directory.ReadWrite.All, Directory.AccessAsUser.All
+ Для приложения Разрешить администраторам недействительными приложений пользователя изъявил: Directory.ReadWrite.All, Directory.AccessAsUser.All

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

## <a name="request-body"></a>Текст запроса
Эта операция не имеет запроса содержимого.

## <a name="response"></a>Ответ

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

##### <a name="response"></a>Ответ
Ниже приведен пример отклика. 
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
  "description": "user: invalidateAllRefreshTokens",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-invalidateallrefreshtokens.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
