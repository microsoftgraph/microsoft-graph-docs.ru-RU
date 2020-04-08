---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ba7d1cb38e1b33d7007cf4613550868d2b634c11
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181373"
---
# <a name="directory-resource-type-deleted-items"></a>Тип ресурса directory (удаленные элементы)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет удаленный элемент в каталоге. После удаления элемент добавляется в "контейнер" удаленных элементов. Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.

В настоящее время функции удаленных элементов поддерживаются только для ресурсов [приложения](application.md), [групп](group.md) и [пользователей](user.md) .

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип | Описание |
|:---------------|:------------|:------------|
|[Получение удаленного элемента](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | Получает свойства удаленного элемента. |
|[Восстановление удаленного элемента](../api/directory-deleteditems-restore.md) |[directoryObject](directoryobject.md)| Восстанавливает недавно удаленный элемент. |
|[Перечисление удаленных элементов](../api/directory-deleteditems-list.md) |Коллекция [directoryObject](directoryobject.md)| Получает список недавно удаленных элементов. |
|[Окончательное удаление элемента](../api/directory-deleteditems-delete.md) | None | Окончательно удаляет элемент. |
|[Список удаленных элементов, принадлежащих пользователю](../api/directory-deleteditems-user-owned.md) | Коллекция [directoryObject](directoryobject.md) | Список элементов каталога, принадлежащих пользователю. |
|[Список ФеатурероллаутполиЦиес](../api/directory-list-featurerolloutpolicies.md) | Коллекция [феатурероллаутполици](featurerolloutpolicy.md) | Получение списка объектов Феатурероллаутполици. |
|[Создание Феатурероллаутполици](../api/directory-post-featurerolloutpolicies.md) | [феатурероллаутполици](featurerolloutpolicy.md) | Создание нового объекта Феатурероллаутполици. |
| [Получение Феатурероллаутполици](../api/featurerolloutpolicy-get.md) | [феатурероллаутполици](featurerolloutpolicy.md) | Получение свойств и связей объекта феатурероллаутполици. |
| [Обновление Феатурероллаутполици](../api/featurerolloutpolicy-update.md) | [феатурероллаутполици](featurerolloutpolicy.md) | Обновление свойств объекта феатурероллаутполици. |
| [Удаление Феатурероллаутполици](../api/featurerolloutpolicy-delete.md) | Нет | Удаление объекта Феатурероллаутполици. |

## <a name="properties"></a>Свойства
| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|String| Уникальный идентификатор объекта, например 12345678-9abc-def0-1234-56789abcde. Ключ. Значение null не допускается. Только для чтения.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|deleteditems|Коллекция [directoryObject](directoryobject.md)| Недавно удаленные элементы. Только для чтения. Допускается значение null.|
|феатурероллаутполиЦиес|Коллекция [феатурероллаутполици](featurerolloutpolicy.md)| Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
