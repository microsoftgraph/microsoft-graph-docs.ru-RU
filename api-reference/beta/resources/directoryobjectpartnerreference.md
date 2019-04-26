---
title: Тип ресурса Директорйобжектпартнерреференце
description: Представляет ссылку на объект каталога в клиенте-партнере. Наследуется от directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 91d33993ea83ea7eba883534efb513fa80287a64
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340854"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>Тип ресурса Директорйобжектпартнерреференце

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ссылку на объект каталога в партнерской организации. Наследуется от [directoryObject](directoryobject.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|description|String| Описание возвращаемого объекта. Только для чтения. |
|displayName|String| Имя возвращаемого объекта каталога, например Group или Application. Только для чтения. |
|Екстерналпартнертенантид|GUID| Идентификатор клиента для партнерского клиента. Только для чтения. |
|id|Строка| Уникальный идентификатор ресурса. Наследуется от [directoryObject](directoryobject.md). Только для чтения. |
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
