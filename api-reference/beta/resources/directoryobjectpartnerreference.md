---
title: Тип ресурса directoryObjectPartnerReference
description: Представляет ссылку на объект каталога в клиентов партнера. Наследуется от directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ba72f70a29e778127454ec3bd4f259331d1fe4c5
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570746"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>Тип ресурса directoryObjectPartnerReference

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет ссылку на объект каталога в партнерской организации. Наследуется от [directoryObject](../resources/directoryobject.md).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|description|Строка| Описание объект, возвращенный. Только для чтения. |
|displayName|Строка| Имя объекта каталога, возвращаемых, такой как группы или приложения. Только для чтения. |
|externalPartnerTenantId|Guid| Идентификатор клиента для клиента партнера. Только для чтения. |
|id|Строка| Уникальный идентификатор для ресурса. Наследуется от [directoryObject](../resources/directoryobject.md). Только для чтения. |
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryobjectpartnerreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
