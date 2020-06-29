---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая закреплена (присоединена) к каналу в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1e113575745e50f52571636f37a7a2d4c93a9924
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909774"
---
# <a name="teamstab-resource-type"></a>Тип ресурса teamsTab

Пространство имен: microsoft.graph



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
|  id              |   string                  |  Идентификатор, который уникальным образом определяет определенный экземпляр вкладки канала. только чтение.     |
|  displayName            |   string                  |  Имя вкладки.     |
|  webUrl          |   string                  |  URL-адрес глубокой ссылки для экземпляра вкладки. Только для чтения.     |
|  configuration        |   [теамстабконфигуратион](teamstabconfiguration.md) |  Контейнер для настраиваемых параметров, применяемых к вкладке. Вкладка считается настроенной только после задания этого свойства.     |

## <a name="relationships"></a>Связи

| Связь | Тип   | Описание |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | Приложение, связанное с вкладкой. Его нельзя изменить после создания вкладки. |

## <a name="json-representation"></a>Представление в формате JSON

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
