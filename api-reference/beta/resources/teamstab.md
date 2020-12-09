---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая закреплена (присоединена) к каналу в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fa675992401c8953b5611739ba69cb0d5688f833
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606955"
---
# <a name="teamstab-resource-type"></a>Тип ресурса teamsTab

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

TeamsTab — это [вкладка](../resources/teamstab.md) , которая закреплена (присоединена) к [каналу](channel.md) в [группе](team.md). 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Вкладки списка в канале](../api/channel-list-tabs.md) | [teamsTab](teamstab.md) | Вкладки со списками, закрепленные по каналу.|
|[Получение вкладки в канале](../api/channel-get-tabs.md) | [teamsTab](teamstab.md) | Получение определенной вкладки, закрепленной в канале.|
|[Добавление вкладки в канал](../api/channel-post-tabs.md) | [teamsTab](teamstab.md) | Добавление вкладки к каналу (ПИН-код).|
|[Вкладка "обновление" в канале](../api/channel-patch-tabs.md) | [teamsTab](teamstab.md) | Обновляет свойства вкладки в канале.|
|[Удаление вкладки из канала](../api/channel-delete-tabs.md) | Нет | Удаление (открепление) вкладки из канала.|
|[Список вкладок в чате](../api/chat-list-tabs.md) | [teamsTab](teamstab.md) | Список вкладок, закрепленных в чате.|
|[Получение вкладки в чате](../api/chat-get-tabs.md) | [teamsTab](teamstab.md) | Получение определенной вкладки, закрепленной в чате.|
|[Добавление вкладки в чат](../api/chat-post-tabs.md) | [teamsTab](teamstab.md) | Добавление вкладки в чат (ПИН-код).|
|[Вкладка "обновление" в чате](../api/chat-patch-tabs.md) | [teamsTab](teamstab.md) | Обновляет свойства вкладки в чате.|
|[Удаление вкладки из чата](../api/chat-delete-tabs.md) | Нет | Удаление (открепление) вкладки из чата.|



## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|  id              |   string                  |  Идентификатор, который уникальным образом определяет определенный экземпляр вкладки канала. только чтение.     |
|  displayName            |   string                  |  Имя вкладки.     |
|  имя (не рекомендуется)      |   string                  |  Имя вкладки.     |
|  Теамсаппид (устаревший)|   string             |  Идентификатор определения приложения вкладки. Это значение нельзя изменить после создания вкладки. Так как это свойство является устаревшим, рекомендуем развернуть **teamsApp** , чтобы получить приложение, связанное с вкладкой. |
|  сортордериндекс  |   string                  |  Индекс заказа, используемого для сортировки вкладок.     |
|  webUrl          |   string                  |  URL-адрес глубокой ссылки для экземпляра вкладки. Только для чтения.     |
|  configuration        |   [теамстабконфигуратион](teamstabconfiguration.md) |  Контейнер для настраиваемых параметров, применяемых к вкладке. Вкладка считается настроенной только после задания этого свойства.     |

## <a name="relationships"></a>Связи

| Связь | Тип   | Описание |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | Приложение, связанное с вкладкой. |

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


