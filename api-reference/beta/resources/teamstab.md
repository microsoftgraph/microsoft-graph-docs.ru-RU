---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая закреплена (присоединена) к каналу в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d4b8bf73499bc2cca2a7497e57e3cce6c8cbe5b9
ms.sourcegitcommit: 0f39f39a1c0300ef013ebd12e4df2b5ba4dabbf8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2020
ms.locfileid: "41559042"
---
# <a name="teamstab-resource-type"></a>Тип ресурса teamsTab

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

TeamsTab — это [вкладка](../resources/teamstab.md) , которая закреплена (присоединена) к [каналу](channel.md) в [группе](team.md). 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Перечисление вкладок](../api/teamstab-list.md) | [teamsTab](teamstab.md) | Перечисление вкладок, закрепленных в канале.|
|[Получение вкладки](../api/teamstab-get.md) | [teamsTab](teamstab.md) | Чтение вкладок, закрепленных в канале.|
|[Добавление вкладки](../api/teamstab-add.md) | [teamsTab](teamstab.md) | Добавление (закрепление) вкладки в канал.|
|[Удаление вкладки](../api/teamstab-delete.md) | Нет | Удаление (открепление) вкладки из канала.|
|[Обновление вкладки](../api/teamstab-update.md) | [teamsTab](teamstab.md) | Обновление свойств вкладки.|


## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|  id              |   строка                  |  Идентификатор, который уникальным образом определяет определенный экземпляр вкладки канала. только чтение.     |
|  displayName            |   string                  |  Имя вкладки.     |
|  name            |   string                  |  Устаревшие Имя вкладки.     |
|  teamsAppId           |   string             |  Идентификатор определения приложения вкладки. Это значение нельзя изменить после создания вкладки.     |
|  сортордериндекс  |   string                  |  Индекс заказа, используемого для сортировки вкладок.     |
|  webUrl          |   string                  |  URL-адрес глубокой ссылки для экземпляра вкладки. Только для чтения.     |
|  конфигурацион        |   [теамстабконфигуратион](teamstabconfiguration.md) |  Контейнер для настраиваемых параметров, применяемых к вкладке. Вкладка считается настроенной только после задания этого свойства.     |

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
