---
title: Добавление вкладки в канал
description: 'Добавляет (закрепляет) вкладку в указанный канал в команде. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5575c4ae9267a968c7381ba4a89b66f9e0e7698d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047541"
---
# <a name="add-tab-to-channel"></a>Добавление вкладки в канал

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Добавляет (закрепляет) [вкладку](../resources/teamstab.md) в указанный [канал](../resources/channel.md) в [команде](../resources/team.md). Соответствующее приложение уже должно быть [установлено в команде](../api/team-list-installedapps.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись) | TeamsTab.Create, TeamsTab.ReadWriteForTeam, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.    |
| Приложение   | TeamsTab.Create.Group*, TeamsTab.Create, TeamsTab.ReadWriteForTeam.All, TeamsTab.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All |

> **Примечание**. Разрешения, помеченные звездочкой (*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).

> **Примечание**. Этот API поддерживает разрешения администратора. Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса

[teamsTab](../resources/teamstab.md).

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `201 Created`.

## <a name="example"></a>Пример

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
{
  "displayName": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
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
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a>См. также

- [Настройка типов вкладок buit-in](/graph/teams-configuring-builtin-tabs)
- [Добавление приложения в команду](team-post-installedapps.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


