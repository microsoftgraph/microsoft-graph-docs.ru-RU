---
title: 'канал: Комплетемигратион'
description: Завершите Перенос внешних сообщений, удалив режим миграции из канала.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 35991987816f65b7a52a80857b00621572fbb793
ms.sourcegitcommit: d9457ac1b8c2e8ac4b9604dd9e116fd547d2bfbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/29/2020
ms.locfileid: "48796551"
---
# <a name="channel-completemigration"></a>канал: Комплетемигратион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Завершите процесс переноса сообщений, удалив `migration mode` из [канала](../resources/channel.md) в команде. `Migration mode` — Это специальное состояние, которое предотвращает некоторые операции, например отправку сообщений и добавление участников, в процессе переноса данных.

После выполнения запроса **комплетемигратион** вы не можете импортировать в команду Дополнительные сообщения. Вы можете добавлять участников в команду после того, как запрос возвращает успешный ответ.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется следующее разрешение. Чтобы узнать больше, *Ознакомьтесь* с [разрешениями](/graph/permissions-reference).

|Тип разрешения      | Разрешение  |
|:--------------------|:---------------------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)  | Не поддерживается.|
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений | Teamwork.Migrate.All|

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{teamId}/channels/{channelId}/completeMigration
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
  "name": "completeMigration_channel"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/completeMigration
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

<!-- uuid: 5793eec6-0e5a-11eb-adc1-0242ac120002
2020-10-14 20:22:11 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "completeMigration_ channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
