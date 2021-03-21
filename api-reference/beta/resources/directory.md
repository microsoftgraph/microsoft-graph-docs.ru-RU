---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4eb1cbdcbf0a1256c2bf2bf0cec35479b8bbc2cc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962625"
---
# <a name="directory-resource-type-deleted-items"></a>Тип ресурса directory (удаленные элементы)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет удаленный элемент в каталоге. После удаления элемент добавляется в "контейнер" удаленных элементов. Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.

В настоящее время функции удаленных элементов поддерживаются только для [приложений,](application.md) [групповых и](group.md) [пользовательских](user.md) ресурсов.

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип | Описание |
|:---------------|:------------|:------------|
|[Получение удаленного элемента](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | Получает свойства удаленного элемента. |
|[Восстановление удаленного элемента](../api/directory-deleteditems-restore.md) |[directoryObject](directoryobject.md)| Восстанавливает недавно удаленный элемент. |
|[Перечисление удаленных элементов](../api/directory-deleteditems-list.md) |Коллекция [directoryObject](directoryobject.md)| Получает список недавно удаленных элементов. |
|[Окончательное удаление элемента](../api/directory-deleteditems-delete.md) | None | Окончательно удаляет элемент. |
|[Список удаленных элементов, которые принадлежат пользователю](../api/directory-deleteditems-user-owned.md) | Коллекция [directoryObject](directoryobject.md) | Списки элементов каталогов, которые принадлежат пользователю. |
|[Функция ListRolloutPolicies](../api/list-featurerolloutpolicies.md) | [коллекция featureRolloutPolicy](featurerolloutpolicy.md) | Извлечение списка объектов featureRolloutPolicy. |
|[Создание featureRolloutPolicy](../api/post-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Создайте новый объект featureRolloutPolicy. |
| [Get featureRolloutPolicy](../api/featurerolloutpolicy-get.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Извлечение свойств и связей объекта featurerolloutpolicy. |
| [Обновление функцииRolloutPolicy](../api/featurerolloutpolicy-update.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Обновление свойств объекта featurerolloutpolicy. |
| [Удаление featureRolloutPolicy](../api/featurerolloutpolicy-delete.md) | Нет | Удаление объекта featureRolloutPolicy. |

## <a name="properties"></a>Свойства
| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|Строка| Уникальный идентификатор объекта, например 12345678-9abc-def0-1234-56789abcde. Ключ. Значение null не допускается. Только для чтения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|deleteditems|Коллекция [directoryObject](directoryobject.md)| Недавно удаленные элементы. Только для чтения. Допускается значение null.|
|featureRolloutPolicies|[коллекция featureRolloutPolicy](featurerolloutpolicy.md)| Допускается значение null.|

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


