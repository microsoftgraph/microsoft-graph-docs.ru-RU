---
title: 'Пользователь: служебное invalidateallrefreshtokens'
description: Делает недействительными все маркеры обновления пользователя, выданные приложениям (а также файлам cookie сеанса в браузере пользователя), путем сброса свойства пользователя **refreshtokensvalidfromdatetime и указывая** к текущей дате и времени. Как правило, эта операция выполняется (пользователем или администратором), если пользователь имеет утерянное или украденное устройство.  Эта операция запрещает доступ к данным в Организации, доступ к которым осуществляется через приложения на устройстве, без необходимости первого входа пользователя в систему. В действительности эта операция приведет к принудительному входу пользователя в систему для всех приложений, для которых они ранее были отправлены, независимо от устройства.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c006787c0d68ae0c6ecbb331a9ff410f957a6f93
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544312"
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

## <a name="request-body"></a>Текст запроса
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
