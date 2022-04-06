---
author: JeremyKelley
description: Ресурс listItemVersion представляет предыдущую версию ресурса ListItem.
ms.date: 09/17/2017
title: ListItemVersion
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 3daffc15f394139301d205c08b02b7a1a57f9d5a
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63722919"
---
# <a name="listitemversion-resource-type"></a>Тип ресурса listItemVersion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **listItemVersion** представляет предыдущую версию ресурса [ListItem](listitem.md).

## <a name="tasks-on-listitemversion-resources"></a>Задачи, которые можно выполнить для ресурсов listItemVersion

Ниже перечислены задачи, доступные для ресурсов listItemVersion.

| Стандартная задача                        | Метод HTTP                                                 |
| :--------------------------------- | :---------------------------------------------------------- |
| [Список версий][version-list]      | `GET /sites/{site-id}/items/{item-id}/versions`             |
| [Получение версии][version-get]         | `GET /sites/{site-id}/items/versions/{version-id}`          |
| [Восстановление версии][version-restore] | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource","keyProperty":"id", "@odata.type": "microsoft.graph.listItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a>Свойства

| Свойство                 | Тип                                                 | Описание                                                             |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | строка                                               | Идентификатор версии. Только для чтения.                                       |
| **lastModifiedBy**;       | [IdentitySet](../resources/identityset.md)           | Удостоверение пользователя, который последним изменил версию. Только для чтения.        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | Дата и время последнего изменения версии. Только для чтения.                 |
| **published**            | [PublicationFacet](../resources/publicationfacet.md) | Указывает состояние публикации конкретной версии. Только для чтения. |

## <a name="relationships"></a>Связи

В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.

| Связь | Тип                                           | Описание                                                              |
| :----------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| **fields**   | [FieldValueSet](../resources/fieldvalueset.md) | Коллекция полей и значений для этой версии элемента списка. |

<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": []
}
-->
