---
title: Добавление вкладки в чат
description: 'Добавляет (пин-коды) вкладку в указанный чат. '
author: subray
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1240f01ee04add3af228a597ab811a8daf8e4780
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777729"
---
# <a name="add-tab-to-chat"></a>Добавление вкладки в чат

Пространство имен: microsoft.graph

Добавьте (пин-код) [вкладку](../resources/teamstab.md) в указанный [чат.](../resources/chat.md) Соответствующее приложение уже должно [быть установлено в чате.](../api/chat-list-installedapps.md)

> **Примечание.** Если чат связан с экземпляром [onlineMeeting,](../resources/onlinemeeting.md) вкладка будет добавлена к собранию.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | TeamsTab.Create, TeamsTab.ReadWriteForChat, TeamsTab.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
| Для приложений                            | TeamsTab.Create, TeamsTab.ReadWriteForChat.All, TeamsTab.ReadWrite.All |


## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /chats/{chat-id}/tabs
```

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса

В орган запроса включаем представление JSON [teamsTab](../resources/teamstab.md).

## <a name="response"></a>Отклик

В случае успешного использования этот метод возвращает код ответа и экземпляр ресурса `201 Created` [teamsTab](../resources/teamstab.md) в теле.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "add_tab_to_chat"
}
-->

```http
POST https://graph.microsoft.com/v1.0/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs
Content-Type: application/json

{
  "displayName": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```


### <a name="response"></a>Отклик

Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsTab"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
  "displayName": "My Contoso Tab",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/entity/com.microsoft.teamspace.tab.web/_djb2_msteams_prefix_193fe248-24e6-478f-a66c-ede9ce6dd547?context=%7b%0d%0a++%22context%22%3a+%22chat%22%2c%0d%0a++%22chatId%22%3a+%2219%3ad65713bc498c4a428c71ef9353e6ce20%40thread.v2%22%2c%0d%0a++%22subEntityId%22%3a+null%0d%0a%7d&tenantId=139d16b4-7223-43ad-b9a8-674ba63c7924"
}
```

## <a name="see-also"></a>См. также

- [Настройка встроенных типов вкладок](/graph/teams-configuring-builtin-tabs)
- [Добавление вкладки в канал](channel-post-tabs.md)
- [Добавление приложения в чат](chat-post-installedapps.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add tab to chat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


