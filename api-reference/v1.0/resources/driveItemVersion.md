---
title: тип ресурса driveItemVersion
description: Представляет определенную версию DriveItem.
ms.localizationpriority: medium
ms.prod: sharepoint
author: JeremyKelley
doc_type: resourcePageType
ms.openlocfilehash: 9dea3f33013c4d6fe0530c4f65253873ec3a1a69
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2021
ms.locfileid: "60354765"
---
# <a name="driveitemversion-resource-type"></a>тип ресурса driveItemVersion

Пространство имен: microsoft.graph

Представляет определенную версию [driveItem](driveitem.md).

Следующие задачи доступны для **ресурсов driveItemVersion.**

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

## <a name="properties"></a>Свойства

|      Имя свойства       |                         Тип                         |                               Описание                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| **id**                   | string                                               | Идентификатор версии. Только для чтения.                                       |
| **lastModifiedBy**;       | [IdentitySet](../resources/identityset.md)           | Удостоверение пользователя, который последним изменил версию. Только для чтения.        |
| **lastModifiedDateTime** | [DateTimeOffset](../resources/timestamp.md)          | Дата и время последнего изменения версии. Только для чтения.                 |
| **publication**          | [PublicationFacet](../resources/publicationfacet.md) | Указывает состояние публикации конкретной версии. Только для чтения. |
| **size**                 | Int64                                                | Указывает размер потока контента для этой версии элемента.  |
| **content**              | Stream                                               | Поток контента для этой версии элемента.                        |

## <a name="instance-attributes"></a>Атрибуты экземпляра

| Имя свойства                     | Тип   | Описание
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.downloadUrl      | string | URL-адрес, который можно использовать для скачивания этой версии контента файла. Проверка подлинности не является обязательным условием, если используется такой URL-адрес. Только для чтения.

>**Примечания:** Это `@microsoft.graph.downloadUrl` недолговечная URL-адресовая ссылка, которая не может быть кэшной. URL-адрес будет доступен в течение короткого времени (1 час), после чего станет недействительным.
>Удаление разрешений на доступ к файлу для пользователя может не сразу сделать URL-адрес недействительным.

## <a name="json-representation"></a>Представление JSON

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
  "size": 12356,

  /* instance annotations */
  "@microsoft.graph.downloadUrl": "url",
}
```


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
