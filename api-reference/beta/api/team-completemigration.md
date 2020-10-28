---
title: 'команда: Комплетемигратион'
description: Завершите Перенос внешних сообщений, удалив из команды режим миграции.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0a3f26727e3e084b3fb0bb95467ffae61f6190a0
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48783038"
---
# <a name="team-completemigration"></a>команда: Комплетемигратион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Завершите процесс переноса сообщений, удалив `migration mode` из [команды](../resources/team.md). `Migration mode` — Это специальное состояние, в котором отменяются определенные операции, например операции отправки и участия в сообщениях во время процесса переноса данных.

После выполнения запроса **комплетемигратион** вы не можете импортировать в команду Дополнительные сообщения. Вы можете добавлять участников в команду после того, как запрос возвращает успешный ответ.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется следующее разрешение. Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешение  |
|:--------------------|:---------------------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)  | Не поддерживается.|
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений | Teamwork.Migrate.All|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{teamId}/completeMigration
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->

<!-- {
  "blockType": "request",
  "name": "completeMigration_team"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/completeMigration
```
<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Отклик

Ниже приведен пример ответа.
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: d945a9a4-0e5b-11eb-adc1-0242ac120002
2020-10-14 20:22:11 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "completeMigration_ team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
