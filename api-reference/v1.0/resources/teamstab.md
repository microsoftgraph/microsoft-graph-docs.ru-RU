---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая прикрепленных (вложенный) канала в группе. '
ms.openlocfilehash: 4e9773fa2e4ea6a114c1f2695906c09d84b3f043
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026288"
---
# <a name="teamstab-resource-type"></a>Тип ресурса teamsTab



TeamsTab — [вкладку](../resources/teamstab.md) , которая прикрепленных (вложенный) [канала](channel.md) в [группы](team.md). 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список вкладок](../api/teamstab-list.md) | [teamsTab](teamstab.md) | Списки вкладок прикрепленных к каналу.|
|[Получить вкладки](../api/teamstab-get.md) | [teamsTab](teamstab.md) | Считывает вкладки, прикрепленных к каналу.|
|[Добавление вкладки](../api/teamstab-add.md) | [teamsTab](teamstab.md) | Добавляет (PIN) вкладки на канал.|
|[Удалить вкладку ""](../api/teamstab-delete.md) | Нет | Удаляет (отключит) вкладки из канала.|
|[Вкладка "обновления"](../api/teamstab-update.md) | [teamsTab](teamstab.md) | Обновляет свойства вкладки.|


## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|  id              |   строка                  |  Идентификатор, который уникальным образом определяет определенный экземпляр канала вкладку чтения только.     |
|  displayName            |   строка                  |  Имя вкладки.     |
|  sortOrderIndex  |   целое                     |  Индекс порядок, используемый для сортировки вкладок     |
|  webUrl          |   string                  |  Прямая ссылка URL-адрес экземпляра вкладки. Только для чтения.     |
|  configuration        |   [teamsTabConfiguration](teamstabconfiguration.md) |  Контейнер для пользовательских параметров, применяемых на вкладке. Вкладка считается настроены только после этого свойства.     |

## <a name="relationships"></a>Связи

| Связь | Тип   | Description |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | Приложения, связанного с вкладки. Это нельзя изменить после создания вкладки. |

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
  "sortOrderIndex": "string",
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

[Настройка типов встроенную вкладку](/graph/teams-configuring-builtin-tabs)
