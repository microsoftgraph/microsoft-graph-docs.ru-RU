---
author: JeremyKelley
ms.date: 09/10/2017
title: baseItem
localization_priority: Normal
description: Ресурс baseItem — это абстрактный ресурс, содержащий общий набор свойств, общий для нескольких других типов ресурсов.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 717426f29b8c466af5799871fcc12cf4cd8bdf65
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239095"
---
# <a name="baseitem-resource-type"></a>Тип ресурса baseItem

Пространство имен: microsoft.graph

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
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItem"
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
| description          | String            | Предоставляет видимое пользователю описание элемента. Необязательный параметр.                             |
| eTag                 | string            | ETag для элемента. Только для чтения.                                                          |
| lastModifiedBy       | [identitySet][]   | Идентификатор пользователя, устройства или приложения, внесшего последние изменения в элемент. Только для чтения. |
| lastModifiedDateTime | dateTimeOffset    | Дата и время последнего изменения элемента. Только для чтения.                                   |
| name                 | string            | Имя элемента. Чтение и запись.                                                      |
| parentReference      | [itemReference][] | Сведения о родительском элементе, если элемент выступает в роли родительского элемента. Чтение и запись.                              |
| webUrl               | строка (url-адрес)      | URL-адрес для отображения ресурса в браузере. Только для чтения.                              |

## <a name="relationships"></a>Связи

| Связь       | Тип     | Описание
|:-------------------|:---------|:---------------------------------------------
| createdByUser      | [user][] | Удостоверение пользователя, создавшего элемент. Только для чтения.
| lastModifiedByUser | [user][] | Удостоверение пользователя, который последним изменил элемент. Только для чтения.

[identitySet]: identityset.md
[itemReference]: itemreference.md
[user]: user.md

## <a name="remarks"></a>Примечания

Тип `baseItem` не предназначен для непосредственного использования.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->

