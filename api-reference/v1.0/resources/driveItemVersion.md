---
title: Тип ресурса DriveItemVersion
description: Ресурс **DriveItemVersion** представляет определенной версии DriveItem.
localization_priority: Normal
ms.openlocfilehash: bfdc38ee7685511fc389300c431f915333deb92b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851690"
---
# <a name="driveitemversion-resource-type"></a>Тип ресурса DriveItemVersion

Ресурс **DriveItemVersion** представляет определенную версию элемента [DriveItem](driveitem.md).


## <a name="tasks-on-driveitemversion-resources"></a>Задачи, которые можно выполнить для ресурсов DriveItemVersion

Ниже перечислены задачи, доступные для ресурсов driveItemVersion.

|            Стандартная задача             |         Метод HTTP         |
| :--------------------------------- | :-------------------------- |
| [List versions][version-list]      | `GET /drive/items/{item-id}/versions`  |
| [Get version][version-get]         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| [Get contents][content-get]        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| [Restore version][version-restore] | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

В примерах в предыдущей таблице используется каталог `/drive`, но также существует много других допустимых запросов.

## <a name="json-representation"></a>Представление в формате JSON

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "@type.aka": "oneDrive.driveItemVersion"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" },
  "size": 12356
}
```

## <a name="properties"></a>Свойства

|      Имя свойства       |                         Тип                         |                               Описание                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | строка                                               | Идентификатор версии. Только для чтения.                                       |
| **lastModifiedBy**;       | [IdentitySet](../resources/identityset.md)           | Удостоверение пользователя, который последним изменил версию. Только для чтения.        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | Дата и время последнего изменения версии. Только для чтения.                 |
| **publication**          | [PublicationFacet](../resources/publicationfacet.md) | Указывает состояние публикации конкретной версии. Только для чтения. |
| **size**                 | Int64                                                | Указывает размер потока контента для этой версии элемента.  |
| **content**              | Stream                                               | Поток содержимого для данной версии элемента.                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
