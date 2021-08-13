---
title: тип ресурса teamsTab
description: 'TeamsTab — это вкладка, закрепленная (присоединенная) к каналу в команде. '
localization_priority: Normal
author: AkJo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e77c6c20705856700717a0312178c5d9fe330df349293920293ebc54019a7409
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54231464"
---
# <a name="teamstab-resource-type"></a>тип ресурса teamsTab

Пространство имен: microsoft.graph



TeamsTab — это [вкладка,](../resources/teamstab.md) закрепленная (присоединенная) к [каналу](channel.md) в [команде.](team.md) 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление вкладок](../api/channel-list-tabs.md) | [teamsTab](teamstab.md) | Перечисление вкладок, закрепленных на канале.|
|[Получение вкладки](../api/channel-get-tabs.md) | [teamsTab](teamstab.md) | Чтение вкладки, закрепленной на канале.|
|[Добавление вкладки](../api/channel-post-tabs.md) | [teamsTab](teamstab.md) | Добавление (закрепление) вкладки на канал.|
|[Обновление вкладки](../api/channel-patch-tabs.md) | [teamsTab](teamstab.md) | Обновление свойств вкладки.|
|[Удаление вкладки](../api/channel-delete-tabs.md) | Нет | Удаление (открепление) вкладки из канала.|


## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|  id              |   строка                  |  Идентификатор, уникальный для определенного экземпляра вкладки канала. Только чтение.     |
|  displayName            |   string                  |  Имя вкладки.     |
|  webUrl          |   string                  |  URL-адрес глубокой ссылки экземпляра вкладки. Только для чтения.     |
|  configuration        |   [teamsTabConfiguration](teamstabconfiguration.md) |  Контейнер для настраиваемой настройки, примененной к вкладке. Вкладка считается настроенной только после заданной настройки этого свойства.     |

## <a name="relationships"></a>Связи

| Связь | Тип   | Описание |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | Приложение, связанное со вкладками. Это невозможно изменить после создания вкладки. |

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

