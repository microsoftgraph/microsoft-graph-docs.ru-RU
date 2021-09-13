---
title: тип ресурса teamsTab
description: 'TeamsTab — это вкладка, закрепленная (присоединенная) к каналу в команде. '
ms.localizationpriority: medium
author: AkJo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 66dfa63b09463fac67b95bf4e635d90ffa4348a7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59066977"
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
|  id              |   string                  |  Идентификатор, уникальный для определенного экземпляра вкладки канала. Только чтение.     |
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

