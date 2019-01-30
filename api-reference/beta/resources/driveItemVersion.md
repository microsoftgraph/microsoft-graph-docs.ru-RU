---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: DriveItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 69c4ed030d090dce9d8bfd8e7ad7a410ad2d4b27
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642025"
---
# <a name="driveitemversion-resource-type"></a>Тип ресурса DriveItemVersion

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **DriveItemVersion** представляет определенную версию элемента [DriveItem](driveitem.md).


## <a name="tasks-on-driveitemversion-resources"></a>Задачи, которые можно выполнить для ресурсов DriveItemVersion

Ниже перечислены задачи, доступные для ресурсов driveItemVersion.

|            Стандартная задача             |         Метод HTTP         |
| :--------------------------------- | :-------------------------- |
| [List versions][version-list]      | `GET /drive/items/{item-id}/versions`  |
| [Get version][version-get]         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| [Get contents][content-get]        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| [Restore version][version-restore] | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

В примерах в предыдущей таблице используется каталог `/drive`, но также существует много других допустимых запросов.

## <a name="json-representation"></a>Представление в формате JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemVersion", "@type.aka": "oneDrive.driveItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a>Свойства

|      Имя свойства       |                         Тип                         |                               Описание                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | Идентификатор версии. Только для чтения.                                       |
| **lastModifiedBy**;       | [IdentitySet](../resources/identityset.md)           | Удостоверение пользователя, который последним изменил версию. Только для чтения.        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | Дата и время последнего изменения версии. Только для чтения.                 |
| **publication**          | [PublicationFacet](../resources/publicationfacet.md) | Указывает состояние публикации конкретной версии. Только для чтения. |
| **size**                 | Int64                                                | Указывает размер потока контента для этой версии элемента.  |

## <a name="relationships"></a>Связи

В таблице ниже определены связи между ресурсом **driveItemVersion** и другими ресурсами.

| Имя связи |  Тип  |            Описание             |
| :---------------- | :----- | :--------------------------------- |
| **content**       | Stream | Поток контента версии. |

<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/driveItemVersion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
