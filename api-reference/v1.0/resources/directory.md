---
title: Тип ресурса directory (удаленные элементы)
description: . Удаленные элементы можно восстановить в течение 30 дней. Через 30 дней элементы удаляются без возможности восстановления.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e5163a50c6c16e9e2d2c6e315e3a701af6da0f88cdc555dcd6b31494ef4e98f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130375"
---
# <a name="directory-resource-type-deleted-items"></a>Тип ресурса directory (удаленные элементы)

Пространство имен: microsoft.graph

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

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|deletedItems|Коллекция [directoryObject](directoryobject.md)| Недавно удаленные элементы. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a>Пример

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/directory
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.directory"}-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
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

