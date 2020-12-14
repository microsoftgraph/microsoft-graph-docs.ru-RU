---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, закрепленная (прикрепленная) к каналу в команде. '
localization_priority: Normal
author: AkJo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8314604d6ed15eeb154ff46c8e3b90f4be4f5cde
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658550"
---
# <a name="teamstab-resource-type"></a>Тип ресурса teamsTab

Пространство имен: microsoft.graph



TeamsTab — [это](../resources/teamstab.md) вкладка, закрепленная (прикрепленная) к [каналу](channel.md) в [команде.](team.md) 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление вкладок](../api/channel-list-tabs.md) | [teamsTab](teamstab.md) | Перечисление вкладок, закрепленных на канале.|
|[Получение вкладки](../api/channel-get-tabs.md) | [teamsTab](teamstab.md) | Чтение вкладки, закрепленной в канале.|
|[Добавление вкладки](../api/channel-post-tabs.md) | [teamsTab](teamstab.md) | Добавление (закрепление) вкладки на канал.|
|[Обновление вкладки](../api/channel-patch-tabs.md) | [teamsTab](teamstab.md) | Обновление свойств вкладки.|
|[Удаление вкладки](../api/channel-delete-tabs.md) | Нет | Удаление (открепление) вкладки из канала.|


## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|  id              |   string                  |  Идентификатор, однозначно определяя определенный экземпляр вкладки канала. Только для чтения.     |
|  displayName            |   string                  |  Имя вкладки.     |
|  webUrl          |   string                  |  URL-адрес глубокой ссылки для экземпляра вкладки. Только для чтения.     |
|  configuration        |   [teamsTabConfiguration](teamstabconfiguration.md) |  Контейнер для настраиваемой настройки, примененной к вкладке. Вкладка считается настроенной только после настройки этого свойства.     |

## <a name="relationships"></a>Связи

| Связь | Тип   | Описание |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | Приложение, связанное со вкладками. Его нельзя изменить после создания вкладки. |

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
  "webUrl": "string",
  "configuration" : "teamsTabConfiguration"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTab resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

## <a name="see-also"></a>См. также

[Настройка встроенных типов вкладок](/graph/teams-configuring-builtin-tabs)

