---
title: Архивация объекта команды
description: 'Архивация указанной команды. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a009dc7214627575b00b2537875e5561b0515d32
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2019
ms.locfileid: "31889921"
---
# <a name="archive-team"></a>Архивация объекта команды

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Архивация указанной [команды](../resources/team.md). Когда команда архивируется, пользователи больше не смогут отправлять и отправлять сообщения на любой канал в команде, изменять имя, описание или другие параметры группы, а в целом вносить большинство изменений в команду.
Изменения членства в команде продолжают разрешены.

Архивация это асинхронная операция. Команда архивируется после успешного завершения асинхронной операции, которая может произойти после ответа от этого API.

Чтобы архивировать группу, группа и [Группа](../resources/group.md) должна иметь владельца.

Чтобы восстановить группу из состояния архивирования, используйте API для архивации. [](team-unarchive.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Group.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Group.ReadWrite.All    |

> **Примечание**. Этот API поддерживает разрешения администратора. Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса
В запросе можно указать __ `shouldSetSpoSiteReadOnlyForMembers` параметр в теле JSON следующим образом.
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
Этот необязательный параметр определяет, нужно ли устанавливать разрешения для участников группы только для чтения на сайте SharePoint Online, связанном с командой. Если задать для него значение false или опустить текст, это приведет к пропущению этого шага.

## <a name="response"></a>Ответ

При успешном запуске архивации этот метод возвращает код `202 Accepted` отклика. Ответ также будет содержать `Location` заголовок, который содержит расположение [теамсасинкоператион](../resources/teamsasyncoperation.md) , созданного для обработки архивации команды. Проверьте состояние операции архивации, выполнив запрос GET к этому расположению.

## <a name="example"></a>Пример
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a>Ответ
Ниже приведен пример ответа.
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-archive.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
