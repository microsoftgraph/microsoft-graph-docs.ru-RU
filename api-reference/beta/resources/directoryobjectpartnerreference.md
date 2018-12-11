---
title: Тип ресурса directoryObjectPartnerReference
description: Представляет ссылку на объект каталога в клиентов партнера. Наследуется от directoryObject.
ms.openlocfilehash: ebdd7380eaa6b59488aca46120339f7175b640fa
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2018
ms.locfileid: "27224129"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>Тип ресурса directoryObjectPartnerReference

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет ссылку на объект каталога в партнерской организации. Наследуется от [directoryObject](directoryobject.md?view=graph-rest-beta).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|описание|Строка| Описание объект, возвращенный. Только для чтения. |
|displayName|Строка| Имя объекта каталога, возвращаемых, такой как группы или приложения. Только для чтения. |
|externalPartnerTenantId|Guid| Идентификатор клиента для клиента партнера. Только для чтения. |
|id|Строка| Уникальный идентификатор для ресурса. Наследуется от [directoryObject](directoryobject.md?view=graph-rest-beta). Только для чтения. |
|objectType|Строка| Тип объекта, который указывает ссылка в партнера для клиентов. Только для чтения. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObjectPartnerReference"
}-->

```json
{
  "description": "string ",
  "displayName": "string",
  "externalPartnerTenantId": "string (identifier)",
  "id": "string (identifier)",
  "objectType": "string"
}
```

## <a name="see-also"></a>См. также

- [Получение объектов каталога из списка идентификаторов](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
