---
title: 'Пользователь: Ревокесигнинсессионс'
description: Делает недействительным все маркеры обновления пользователя, выданные приложениям (а также файлам cookie сеанса в браузере пользователя), путем сброса свойства пользователя **сигнинсессионсвалидфромдатетиме** к текущей дате и времени.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 607b89201958ec2c8062109e2e02b1749b1c96ef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536595"
---
# <a name="user-revokesigninsessions"></a>Пользователь: Ревокесигнинсессионс

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Делает недействительными все маркеры обновления, выданные приложениям для пользователя (а также файлы cookie сеансов в браузере пользователя), путем сброса свойства пользователя **сигнинсессионсвалидфромдатетиме** к текущей дате и времени. Как правило, эта операция выполняется (пользователем или администратором), если пользователь имеет утерянное или украденное устройство. Эта операция запрещает доступ к данным Организации через приложения на устройстве, требуя от пользователя повторного входа во все приложения, которые ранее были отосланы, независимо от устройства.

Если приложение пытается активировать маркер делегированного доступа для этого пользователя с помощью недействительного маркера обновления, приложение получит ошибку. В этом случае приложению потребуется получить новый маркер обновления, выполнив запрос к конечной точке авторизации, которая вынуждает пользователя выполнить вход.

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

## <a name="request-body"></a>Текст запроса
В этой операции нет содержимого запроса.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример
В приведенном ниже примере показано, как вызывать этот API.

##### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "user_revokesigninsessionss"
}-->
```http
POST https://graph.microsoft.com/beta/me/revokeSignInSessions
```

##### <a name="response"></a>Ответ
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
    "Error: /api-reference/beta/api/user-revokesigninsessions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
