---
title: Архивация команды
description: 'Архивация указанной команды. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8d7631524350c37a79913bbb4b37d0b6e9ee4651
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452609"
---
# <a name="archive-team"></a>Архивация команды

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Архивация указанной [команды](../resources/team.md). При архивации команды пользователь больше не сможет отправлять сообщения в любой канал команды или присваивать сообщениям отметку "Нравится", изменять название команды, описание, другие параметры и в целом вносить большинство изменений в команду.
Изменение участия в команде по-прежнему допускается.

Архивация — это асинхронная операция. Команда архивируется после успешного завершения асинхронной операции, которая может выполняться после отклика этого API.

Чтобы архивировать команду, у команды и [группы](../resources/group.md) должен быть владелец.

Чтобы восстановить команду из архивированного состояния, используйте API для [распаковки](team-unarchive.md).

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
В запросе можно _при необходимости_ включить параметр `shouldSetSpoSiteReadOnlyForMembers` в текст JSON следующим образом.
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
Этот необязательный параметр определяет, следует ли для участников команды задать разрешения только для чтения на сайте Sharepoint Online, связанном с командой. Если присвоить ему значение false или не указать текст, этот этап будет пропущен.

## <a name="response"></a>Ответ

Если архивация начата успешно, этот метод возвращает код отклика `202 Accepted`. Отклик также будет содержать заголовок `Location`, в котором указывается расположение ресурса [teamsAsyncOperation](../resources/teamsasyncoperation.md), созданного для обработки архивации команды. Проверьте состояние операции архивации, выполнив запрос GET для этого расположения.

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
#### <a name="response"></a>Отклик
Ниже приведен пример отклика.
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
  "suppressions": []
}
-->
