---
author: JeremyKelley
description: Ресурс baseItem — это абстрактный ресурс, содержащий общий набор свойств, совместно используемых несколькими другими типами ресурсов.
ms.date: 09/10/2017
title: baseItem
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: 770106991a8e2008245a4a7665155eafe6ad7216
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944957"
---
# <a name="baseitem-resource-type"></a>Тип ресурса baseItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**baseItem** — это абстрактный ресурс, который содержит стандартный набор свойств, также используемых несколькими другими типами ресурсов. Ниже перечислены ресурсы, производные от ресурса **baseItem**.

* [drive](drive.md)
* [driveItem](driveitem.md)
* [site](site.md)
* [sharedDriveItem](shareddriveitem.md)

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **baseItem** в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseItem",
  "abstract": true
}-->

```json
{
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a>Свойства

| Свойство             | Тип              | Описание                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| id                   | string            | Уникальный идентификатор диска. Только для чтения.                                         |
| createdBy            | [identitySet][]   | Идентификатор пользователя, устройства или приложения, создавшего элемент. Только для чтения.        |
| createdDateTime      | dateTimeOffset    | Дата и время создания элемента. Только для чтения.                                             |
| eTag                 | string            | ETag для элемента. Только для чтения.                                                          |
| lastModifiedBy       | [identitySet][]   | Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения. |
| lastModifiedDateTime | dateTimeOffset    | Дата и время последнего изменения элемента. Только для чтения.                                   |
| name                 | string            | Имя элемента. Чтение и запись.                                                      |
| parentReference      | [itemReference][] | Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.                              |
| webUrl               | строка (url-адрес)      | URL-адрес для отображения ресурса в браузере. Только для чтения.                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a>Примечания

Тип `baseItem` не предназначен для непосредственного использования.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem",
  "suppressions": []
}
-->


