---
title: Тип ресурса teamsTab
description: 'TeamsTab — это вкладка, которая закреплена (присоединена) к каналу в группе. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 181d2fd23ff922709b3e098f6069adf300ad3928
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456985"
---
# <a name="teamstab-resource-type"></a>Тип ресурса teamsTab



TeamsTab — это [вкладка](../resources/teamstab.md) , которая закреплена (присоединена) к [каналу](channel.md) в [группе](team.md). 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список вкладок](../api/teamstab-list.md) | [teamsTab](teamstab.md) | Список вкладок, закрепленных в канале.|
|[Получение вкладки](../api/teamstab-get.md) | [teamsTab](teamstab.md) | Считывает вкладку, закрепленную в канале.|
|[Добавление вкладки](../api/teamstab-add.md) | [teamsTab](teamstab.md) | Добавляет в канал вкладку (ПИН-код).|
|[Удалить вкладку](../api/teamstab-delete.md) | Нет | Удаляет (открепляет) вкладку из канала.|
|[Обновление вкладки](../api/teamstab-update.md) | [teamsTab](teamstab.md) | Обновляет свойства вкладки.|


## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---------------|:--------|:----------|
|  id              |   строка                  |  Идентификатор, который уникальным образом определяет определенный экземпляр вкладки канала. только чтение.     |
|  displayName            |   string                  |  Имя вкладки.     |
|  webUrl          |   string                  |  URL-адрес глубокой ссылки для экземпляра вкладки. Только для чтения.     |
|  конфигурацион        |   [Теамстабконфигуратион](teamstabconfiguration.md) |  Контейнер для настраиваемых параметров, применяемых к вкладке. Вкладка считается настроенной только после задания этого свойства.     |

## <a name="relationships"></a>Связи

| Отношение | Тип   | Описание |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md) | Приложение, связанное с вкладкой. Его нельзя изменить после создания вкладки. |

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
