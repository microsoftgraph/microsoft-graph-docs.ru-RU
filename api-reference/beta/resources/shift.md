---
title: Тип ресурса shift
description: Смена — это единица запланированных трудозатрат в расписании.
author: aaku
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5d17e9610ce4e2f5de82585a8281aab9fdfbf538
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63720817"
---
# <a name="shift-resource-type"></a>Тип ресурса shift

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Единица запланированных трудозатрат в [расписании](schedule.md). 

## <a name="methods"></a>Методы

| Метод                                         | Возвращаемый тип                  | Описание                                |
| :--------------------------------------------- | :--------------------------- | :----------------------------------------- |
| [Создание смены](../api/schedule-post-shifts.md) | [shift](shift.md)            | Создание объекта `shift`.                      |
| [Перечисление смен](../api/schedule-list-shifts.md)  | Коллекция [shift](shift.md) | Получение списка объектов `shifts` в расписании. |
| [Получение смены](../api/shift-get.md)               | [shift](shift.md)            | Получение `shift` по идентификатору.                       |
| [Замена смены](../api/shift-put.md)           | [shift](shift.md)            | Замена объекта `shift`.                         |
| [Удаление смены](../api/shift-delete.md)         | Нет                         | Удаление объекта `shift` из расписания.        |

## <a name="properties"></a>Свойства

| Свойство             | Тип                          | Описание                                                                                                                                                                                                                         |
| -------------------- | ----------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| id                   | `string`                      | Идентификатор объекта `shift`.                                                                                                                                                                                                                  |
| userId               | `string`                      | Идентификатор пользователя, назначенного объекту `shift`. Обязательный элемент.                                                                                                                                                                                   |
| schedulingGroupId    | `string`                      | Идентификатор группы планирования, частью которой является объект `shift`. Обязательный элемент.                                                                                                                                                                        |
| sharedShift          | [shiftItem](shiftitem.md)     | Общая версия объекта `shift`, доступная для просмотра как сотрудникам, так и руководителям. Обязательный элемент.                                                                                                                                       |
| draftShift           | [shiftItem](shiftitem.md)     | Черновая версия объекта `shift`, доступная для просмотра руководителями. Обязательный элемент.                                                                                                                                                           |
| createdDateTime      | `DateTimeOffset`              | Метка времени создания объекта `shift`. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
| lastModifiedDateTime | `DateTimeOffset`              | Метка времени последнего обновления объекта `shift`. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.  |
| lastModifiedBy       | [identitySet](identityset.md) | Учетная запись, которая последней обновила этот объект `shift`.                                                                                                                                                                                        |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shift"
}-->

```json
{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedShift": {"@odata.type":"microsoft.graph.shiftItem"},
  "draftShift": {"@odata.type":"microsoft.graph.shiftItem"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "shift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
