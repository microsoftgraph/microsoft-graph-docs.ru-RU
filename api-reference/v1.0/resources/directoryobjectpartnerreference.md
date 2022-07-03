---
title: Тип ресурса directoryObjectPartnerReference
description: Представляет ссылку на объект каталога в клиенте партнера. Наследуется от directoryObject.
author: keylimesoda
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 10365c3a7a2dbc559cfd090710e99998e1f50c54
ms.sourcegitcommit: 6a4e81d2b8e7447771c9060998c7e1cc18a57902
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/03/2022
ms.locfileid: "66609698"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>Тип ресурса directoryObjectPartnerReference

Пространство имен: microsoft.graph

Представляет ссылку на объект каталога в партнерской организации. Наследуется от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0&preserve-view=true).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|description|String| Описание возвращаемого объекта. Только для чтения. |
|displayName|String| Имя возвращаемого объекта каталога, например группа или приложение. Только для чтения. |
|externalPartnerTenantId|Guid| Идентификатор клиента партнера. Только для чтения. |
|id|String| Уникальный идентификатор ресурса. Наследуется от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0&preserve-view=true). Только для чтения. |
|Objecttype|String| Тип объекта, на который указывает ссылка, в клиенте партнера. Только для чтения. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObjectPartnerReference"
}-->

```json
{
  "description": "String ",
  "displayName": "String",
  "externalPartnerTenantId": "String (identifier)",
  "id": "String (identifier)",
  "objectType": "String"
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
