---
title: Тип ресурса Аудиораутингграуп
description: В группе маршрутизации звука хранится частный звуковой маршрут между участниками в составе многоадресной беседы. Источник — сам участник, а приемники являются подмножеством других участников многочастой беседы.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e7fc7de5b5caaa2f4079c453f9cd855a42577cb8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544003"
---
# <a name="audioroutinggroup-resource-type"></a>Тип ресурса Аудиораутингграуп

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В группе маршрутизации звука хранится частный звуковой маршрут между участниками в составе многоадресной беседы. Источник — сам участник, а приемники являются подмножеством других участников многочастой беседы.

> **Примечание:** [Конфигуремиксер](../api/participant-configuremixer.md) не включает ни одного маршрута, он предназначен для всего вызова для настройки уровней громкости для комбинаций исходного приемника.

## <a name="methods"></a>Методы

| Метод                                                  | Возвращаемый тип                               | Описание                                  |
|:--------------------------------------------------------|:------------------------------------------|:---------------------------------------------|
| [Получение Аудиораутингграуп](../api/audioroutinggroup-get.md)| [audioRoutingGroup](audioroutinggroup.md) | Чтение свойств и связей объекта Аудиораутингграуп.|
| [Обновление](../api/audioroutinggroup-update.md)            | [audioRoutingGroup](audioroutinggroup.md) | Обновление списка получателей.                       |
| [Удаление](../api/audioroutinggroup-delete.md)            | Нет                                      | Удаление группы маршрутизации звука.              |

## <a name="properties"></a>Свойства

| Свойство      | Тип              | Описание                                                          |
| :----------   | :---------------- | :--------------------------------------------------------------------|
| id            | String            | Только для чтения. Создается сервером.                                         |
| приемники     | Коллекция String | Список идентификаторов участников.                                   |
| Раутингмоде   | String            | Режим группы маршрутизации.  Возможные значения: `oneToOne`, `multicast`.   |
| sources       | Коллекция String | Список идентификаторов участников исходного участника.                                      |

> **Примечание:** Режим маршрутизации определяет ограничения для источников и получателей. Поддерживаются только следующие группы маршрутизации.
> - `oneToOne`— у источников и приемников есть только один участник.
> - `multicast`Источник имеет одного участника, но существует несколько получателей. Список получателей можно обновить.

> **Примечание:** Если вы создаете множество групп маршрутизации звука (например, Bot для каждого участника), пересылается только звук главных 4 главных динамиков. Это означает, что даже если пользователь настроил группу маршрутизации аудио, если динамики не хватает громкости в основном микшере, то он/она не может быть слышна с помощью Bot, даже если для этого динамика и для этого динамика достаточно частной группы звука.

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление в формате JSON

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
