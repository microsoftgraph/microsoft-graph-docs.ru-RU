---
title: Тип ресурса directoryObjectPartnerReference
description: Представляет ссылку на объект каталога в клиентов партнера. Наследуется от directoryObject.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 17bab72fad3e03b843975ae62261fac9c09af791
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918541"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>Тип ресурса directoryObjectPartnerReference

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет ссылку на объект каталога в партнерской организации. Наследуется от [directoryObject](directoryobject.md?view=graph-rest-beta).

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|описание|String| Описание объект, возвращенный. Только для чтения. |
|displayName|String| Имя объекта каталога, возвращаемых, такой как группы или приложения. Только для чтения. |
|externalPartnerTenantId|Guid| Идентификатор клиента для клиента партнера. Только для чтения. |
|id|String| Уникальный идентификатор для ресурса. Наследуется от [directoryObject](directoryobject.md?view=graph-rest-beta). Только для чтения. |
|objectType|String| Тип объекта, который указывает ссылка в партнера для клиентов. Только для чтения. |

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
