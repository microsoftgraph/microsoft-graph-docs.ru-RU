---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: ListItemVersion
localization_priority: Normal
ms.openlocfilehash: 0ffdda98d941ef197bd956146ba796ace037cb8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849625"
---
# <a name="listitemversion-resource-type"></a>Тип ресурса listItemVersion

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Ресурс **listItemVersion** представляет предыдущую версию ресурса [ListItem](listitem.md).

## <a name="tasks-on-listitemversion-resources"></a>Задачи, которые можно выполнить для ресурсов listItemVersion

Ниже перечислены задачи, доступные для ресурсов listItemVersion.

|            Стандартная задача             |         Метод HTTP         |
| :--------------------------------- | :-------------------------- |
| [List versions][version-list]      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| [Get version][version-get]         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| [Restore version][version-restore] | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a>Представление в формате JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.listItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

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

|      Имя свойства       |                         Тип                         |                               Описание                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | строка                                               | Идентификатор версии. Только для чтения.                                       |
| **lastModifiedBy**;       | [IdentitySet](../resources/identityset.md)           | Удостоверение пользователя, который последним изменил версию. Только для чтения.        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | Дата и время последнего изменения версии. Только для чтения.                 |
| **published**            | [PublicationFacet](../resources/publicationfacet.md) | Указывает состояние публикации конкретной версии. Только для чтения. |


## <a name="relationships"></a>Связи

В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.

| Имя связи |                      Тип                      |                               Описание                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| **fields**        | [FieldValueSet](../resources/fieldvalueset.md) | Коллекция полей и значений для этой версии элемента списка. |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
