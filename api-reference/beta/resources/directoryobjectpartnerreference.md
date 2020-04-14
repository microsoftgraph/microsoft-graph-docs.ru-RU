---
title: Тип ресурса Директорйобжектпартнерреференце
description: Представляет ссылку на объект каталога в клиенте-партнере. Наследуется от directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1e98395b627489b73a3638c88afc91b9edd86e54
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442986"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>Тип ресурса Директорйобжектпартнерреференце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ссылку на объект каталога в партнерской организации. Наследуется от [directoryObject](directoryobject.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|description|String| Описание возвращаемого объекта. Только для чтения. |
|displayName|Строка| Имя возвращаемого объекта каталога, например Group или Application. Только для чтения. |
|екстерналпартнертенантид|GUID| Идентификатор клиента для партнерского клиента. Только для чтения. |
|id|String| Уникальный идентификатор ресурса. Наследуется от [directoryObject](directoryobject.md). Только для чтения. |
|objectType|String| Тип упоминаемого объекта в партнерской клиенте. Только для чтения. |

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
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
