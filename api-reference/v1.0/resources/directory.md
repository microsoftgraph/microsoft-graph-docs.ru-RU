---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9f337a8a516dbd1bc3bd772a52f74000d412c071
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59072556"
---
# <a name="directory-resource-type"></a>Тип ресурса каталога

Пространство имен: microsoft.graph

Представляет удаленный элемент в каталоге. После удаления элемент добавляется в "контейнер" удаленных элементов. Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.

В настоящее время функции удаленных элементов поддерживаются только для [приложений,](application.md) [групповых](group.md)и [пользовательских](user.md) ресурсов.

Наследует от [объекта](entity.md).

## <a name="methods"></a>Методы

| Метод         | Возвращаемый тип | Описание |
|:---------------|:------------|:------------|
|[Получение удаленного элемента](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | Получает свойства удаленного элемента. |
|[Восстановление удаленного элемента](../api/directory-deleteditems-restore.md) |[directoryObject](directoryobject.md)| Восстанавливает недавно удаленный элемент. |
|[Перечисление удаленных элементов](../api/directory-deleteditems-list.md) |Коллекция [directoryObject](directoryobject.md)| Получает список недавно удаленных элементов. |
|[Окончательное удаление элемента](../api/directory-deleteditems-delete.md) | None | Окончательно удаляет элемент. |
|[Список удаленных элементов, которые принадлежат пользователю](../api/directory-deleteditems-user-owned.md) | Коллекция [directoryObject](directoryobject.md) | Списки элементов каталогов, которые принадлежат пользователю. |


## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|Строка| Уникальный идентификатор объекта; например, `12345678-9abc-def0-1234-56789abcde` . Ключ. Значение null не допускается. Только для чтения. Наследуется от [сущности](entity.md).|


## <a name="relationships"></a>Отношения

| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|administrativeUnits|[коллекция administrativeUnit](administrativeunit.md)| Концептуальный контейнер для объектов каталога пользователей и групп.|
|deletedItems|Коллекция [directoryObject](directoryobject.md)| Недавно удаленные элементы. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "@odata.type": "#microsoft.graph.directory"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

