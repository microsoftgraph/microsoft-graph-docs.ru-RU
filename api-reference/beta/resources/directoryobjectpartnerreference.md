---
title: тип ресурса directoryObjectPartnerReference
description: Представляет ссылку на объект каталога в клиенте-партнере. Наследуется от directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 8b9d6a8826c38171dc7b32c281c371e841906f82
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761563"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>тип ресурса directoryObjectPartnerReference

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ссылку на объект каталога в организации-партнере. Наследуется от [directoryObject](directoryobject.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|description|String| Описание возвращенного объекта. Только для чтения. |
|displayName|String| Имя возвращаемого объекта каталога, например группы или приложения. Только для чтения. |
|externalPartnerTenantId|Guid| Идентификатор клиента для клиента-партнера. Только для чтения. |
|id|String| Уникальный идентификатор ресурса. Наследуется от [directoryObject](directoryobject.md). Только для чтения. |
|objectType|String| Тип ссылаемого объекта в клиенте-партнере. Только для чтения. |

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

- [Получение объектов каталога из списка идентификаторов](../api/directoryobject-getbyids.md)

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
