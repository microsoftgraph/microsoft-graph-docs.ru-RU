---
title: тип ресурса directoryObjectPartnerReference
description: Представляет ссылку на объект каталога в клиенте-партнере. Наследуется от directoryObject.
author: keylimesoda
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 17356a5e865fceb9da49447064d141120387328e
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854339"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>тип ресурса directoryObjectPartnerReference

Пространство имен: microsoft.graph

Представляет ссылку на объект каталога в организации-партнере. Наследуется от [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|description|Строка| Описание возвращенного объекта. Только для чтения. |
|displayName|String| Имя возвращаемого объекта каталога, например группы или приложения. Только для чтения. |
|externalPartnerTenantId|GUID| Идентификатор клиента для клиента-партнера. Только для чтения. |
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
