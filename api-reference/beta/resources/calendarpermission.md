---
title: Тип ресурса Календарпермиссион
description: Разрешения пользователя, к которому открыт общий доступ к календарю.
localization_priority: Normal
author: sochowdh
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5d19a1738d3369f2d910dd590062016acf3047ab
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950453"
---
# <a name="calendarpermission-resource-type"></a>Тип ресурса Календарпермиссион

Разрешения пользователя, к которому открыт общий доступ к календарю. 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение Календарпермиссион](../api/calendarpermission-get.md) | [календарпермиссион](calendarpermission.md) | Чтение свойств и связей объекта Календарпермиссион. |
| [Update](../api/calendarpermission-update.md) | [календарпермиссион](calendarpermission.md) | Обновление объекта Календарпермиссион. |
| [Delete](../api/calendarpermission-delete.md) | Нет. | Удаление объекта Календарпермиссион. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|алловедролес|Коллекция строк| Список разрешенных для общего доступа уровней разрешений для календаря. Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|
|emailAddress|[emailAddress](emailaddress.md)| Представляет общую папку, у которой есть доступ к календарю. Для общего доступа к общему ресурсу "Моя организация" свойство **Address** имеет значение null. |
|id|String| Уникальный идентификатор пользователя (общего доступа), с которым открыт общий доступ к календарю. Только для чтения.|
|исинсидеорганизатион|Логический| Значение true, если пользователь в контексте (Share) находится в той же организации, что и владелец календаря.|
|"несъемный"|Логический| `True`, если пользователь может быть удален из списка общих папок для указанного календаря, `false` в противном случае. Пользователь "Моя организация" определяет разрешения, которые пользователи в организации имеют в указанном календаре. Вы не можете удалить "Моя организация" как общий доступ к календарю.|
|role|календарролетипе| Текущий уровень разрешений общего календаря. Возможные значения: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.calendarPermission",
  "keyProperty": "id"
}-->

```json
{
  "allowedRoles": ["string"],
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "id": "String (identifier)",
  "isInsideOrganization": "boolean",
  "isRemovable": "boolean",
  "role": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendarPermission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->