---
title: Тип ресурса audioRoutingGroup
description: Аудио группы маршрутизации хранит закрытый звука маршрута между участниками в многосторонней беседе. Источник — это участник самого и приемники являются подмножеством других участников в многосторонней беседе.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e7fc7de5b5caaa2f4079c453f9cd855a42577cb8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509625"
---
# <a name="audioroutinggroup-resource-type"></a>Тип ресурса audioRoutingGroup

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Аудио группы маршрутизации хранит закрытый звука маршрута между участниками в многосторонней беседе. Источник — это участник самого и приемники являются подмножеством других участников в многосторонней беседе.

> **Примечание:** [ConfigureMixer](../api/participant-configuremixer.md) не затрагивает все маршруты, для всей продолжительности вызова для настройки громкость сочетания приемника источника.

## <a name="methods"></a>Методы

| Метод                                                  | Возвращаемый тип                               | Описание                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [Получение audioRoutingGroup](../api/audioroutinggroup-get.md)| [audioRoutingGroup](audioroutinggroup.md) | Чтение свойства и связи объекта audioRoutingGroup.|
| [Update](../api/audioroutinggroup-update.md)            | [audioRoutingGroup](audioroutinggroup.md) | Обновление списка получателей.                       |
| [Delete](../api/audioroutinggroup-delete.md)            | Нет                                      | Удаление звука группы маршрутизации.              |

## <a name="properties"></a>Свойства

| Свойство      | Тип              | Описание                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| id            | String            | Только для чтения. Сервер, созданный.                                         |
| Приемники     | string collection | Список получения участников идентификаторы.                                   |
| routingMode   | String            | Режим группы маршрутизации.  Возможные значения: `oneToOne`, `multicast`.   |
| sources       | string collection | Список идентификаторов участников источника.                                      |

> **Примечание:** Режим маршрутизации определяет ограничения на доступ к источникам и приемников. Поддерживаются только следующие группы маршрутизации.
> - `oneToOne`-источники и приемники имеют только одному участнику.
> - `multicast`-источник имеет один участник, но имеется несколько приемников. Список приемники могут быть обновлены.

> **Примечание:** При создании количество аудио маршрутизации групп (например робот каждого участника), пересылается только звук верхней 4 доминирующий динамики. Это означает даже при использовании настраиваемого звука группу маршрутизации, если динамик не громкость, в главном Микшер, он/она не удается Херд с робот, даже при наличии закрытый звука группы для этого динамика и робот.

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioRoutingGroup"
}-->
```json
{
  "id": "String (identifier)",
  "receivers": [ "String" ],
  "routingMode": "oneToOne | multicast",
  "sources": [ "String" ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioRoutingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audioroutinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
