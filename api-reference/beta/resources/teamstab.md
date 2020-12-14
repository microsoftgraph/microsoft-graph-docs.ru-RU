---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, закрепленная (прикрепленная) к каналу в команде. '
localization_priority: Normal
author: AkJo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 38351b0bde174b03f0e01392e7c8ec9c4df0db44
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660116"
---
# <a name="teamstab-resource-type"></a>Тип ресурса teamsTab

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

TeamsTab — [это](../resources/teamstab.md) вкладка, закрепленная (прикрепленная) к [каналу](channel.md) в [команде.](team.md) 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список вкладок на канале](../api/channel-list-tabs.md) | [teamsTab](teamstab.md) | Перечисление вкладок, закрепленных на канале.|
|[Получение вкладки на канале](../api/channel-get-tabs.md) | [teamsTab](teamstab.md) | Получение определенной вкладки, закрепленной на канале.|
|[Добавление вкладки в канал](../api/channel-post-tabs.md) | [teamsTab](teamstab.md) | Добавление (закрепление) вкладки на канал.|
|[Вкладка "обновление" на канале](../api/channel-patch-tabs.md) | [teamsTab](teamstab.md) | Обновляет свойства вкладки на канале.|
|[Удаление вкладки из канала](../api/channel-delete-tabs.md) | Нет | Удаление (открепление) вкладки из канала.|
|[Список вкладок в чате](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | Список вкладок, закрепленных в чате.|
|[Получить вкладку в чате](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | Получите определенную вкладку, закрепленную в чате.|
|[Добавление вкладки в чат](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | Добавление (закрепление) вкладки в чат.|
|[Вкладка "Обновление" в чате](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | Обновление свойств вкладки в чате.|
|[Удаление вкладки из чата](../api/chat-delete-tabs.md) | Нет | Удалите (открепите) вкладку из чата.|



## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|  id              |   string                  |  Идентификатор, однозначно определяя определенный экземпляр вкладки канала. Только для чтения.     |
|  displayName            |   string                  |  Имя вкладки.     |
|  name (неподготовленное)      |   Строка                  |  Имя вкладки.     |
|  teamsAppId (неименовее)|   Строка             |  Идентификатор определения приложения для вкладки. Это значение нельзя изменить после создания вкладки. Так как это свойство является неподготовленным, мы рекомендуем развернуть **teamsApp,** чтобы получить приложение, связанное с вкладкой. |
|  sortOrderIndex  |   Строка                  |  Индекс порядка, используемого для сортировки вкладок.     |
|  webUrl          |   string                  |  URL-адрес глубокой ссылки для экземпляра вкладки. Только для чтения.     |
|  configuration        |   [teamsTabConfiguration](teamstabconfiguration.md) |  Контейнер для настраиваемой настройки, примененной к вкладке. Вкладка считается настроенной только после настройки этого свойства.     |

## <a name="relationships"></a>Связи

| Связь | Тип   | Описание |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | Приложение, связанное со вкладками. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.


<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.teamsTab"
}-->

```json
{
  "id": "string",
  "displayName": "string",
  "teamsAppId": "string",
  "sortOrderIndex": "string",
  "webUrl": "string",
  "configuration": "teamsTabConfiguration",
  "name": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

## <a name="see-also"></a>См. также

[Настройка встроенных типов вкладок](/graph/teams-configuring-builtin-tabs)


