---
title: Тип ресурса DriveItemVersion
description: Ресурс **DriveItemVersion** представляет определенную версию DriveItem.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: resourcePageType
ms.openlocfilehash: d015175df3f4fb91d6a91dce7cf5b10714f6d1988044e9c98c81fcd5c3dd5369
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54135262"
---
# <a name="driveitemversion-resource-type"></a>Тип ресурса DriveItemVersion

Пространство имен: microsoft.graph

Ресурс **DriveItemVersion** представляет определенную версию элемента [DriveItem](driveitem.md).


## <a name="tasks-on-driveitemversion-resources"></a>Задачи, которые можно выполнить для ресурсов DriveItemVersion

Ниже перечислены задачи, доступные для ресурсов driveItemVersion.

|            Стандартная задача             |         Метод HTTP         |
| :--------------------------------- | :-------------------------- |
| [Список версий][version-list]      | `GET /drive/items/{item-id}/versions`  |
| [Получение версии][version-get]         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| [Get contents][content-get]        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| [Восстановление версии][version-restore] | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

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
  "@type.aka&quot;: &quot;oneDrive.driveItemVersion"
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
| **публикация**          | [PublicationFacet](../resources/publicationfacet.md) | Указывает состояние публикации конкретной версии. Только для чтения. |
| **size**                 | Int64                                                | Указывает размер потока контента для этой версии элемента.  |
| **content**              | Stream                                               | Поток контента для этой версии элемента.                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->

