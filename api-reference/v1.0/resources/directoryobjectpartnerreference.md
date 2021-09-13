---
title: тип ресурса directoryObjectPartnerReference
description: Представляет ссылку на объект каталога в клиенте-партнере. Наследуется от directoryObject.
author: keylimesoda
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 35cc8be163a9bbbbcdf9330d6b6cf861673e7edf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123793"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>тип ресурса directoryObjectPartnerReference

Пространство имен: microsoft.graph

Представляет ссылку на объект каталога в организации-партнере. Наследуется от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|description|String| Описание возвращенного объекта. Только для чтения. |
|displayName|Строка| Имя возвращаемого объекта каталога, например группы или приложения. Только для чтения. |
|externalPartnerTenantId|Guid| Идентификатор клиента для клиента-партнера. Только для чтения. |
|id|String| Уникальный идентификатор ресурса. Наследуется от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0). Только для чтения. |
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
