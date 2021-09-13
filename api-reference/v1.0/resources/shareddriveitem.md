---
author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
ms.localizationpriority: medium
description: Ресурс sharedDriveItem возвращается при использовании API Shares для доступа к общему driveItem.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e425d8d243722ffa29b9ffcedfaae566508d8f57
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59066998"
---
# <a name="shareddriveitem-resource-type"></a>Тип ресурса SharedDriveItem

Пространство имен: microsoft.graph

Ресурс **sharedDriveItem** возвращается, если для доступа к общему элементу [driveItem](driveitem.md) используется API [Shares](../api/shares-get.md).

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса **sharedDriveItem** в формате JSON.

Ресурс **sharedDriveItem** является производным от ресурса [**baseItem**](baseitem.md) и наследует его свойства.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItem",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
  "id": "string",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },

  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "list": { "@odata.type": "microsoft.graph.list" },
  "listItem": { "@odata.type": "microsoft.graph.listItem" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a>Свойства

| Свойство | Тип                          | Описание                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| id       | Строка                        | Уникальный идентификатор для общего ресурса, к которому предоставляется доступ.              |
| name     | String                        | Отображаемое имя общего элемента.                             |
| owner    | [IdentitySet](identityset.md) | Сведения о владельце общего элемента, ставшего объектом ссылки. |

## <a name="relationships"></a>Связи

| Имя связи | Тип                | Описание
| ------------------|:--------------------|:-----------------------------------
| **driveItem**     | [**driveItem**][driveItem]   | Используется для доступа к базовому объекту **driveItem**
| **list**          | [**список**][list]        | Используется для доступа к базовому объекту **list**
| **listItem**      | [**listItem**][listItem]    | Используется для доступа к базовому объекту **listItem**
| **permission**    | [**разрешение**][permission] | Используется для доступа к **разрешению,** представляющим пусковую ссылку общего доступа
| **site**          | [**site**][site]        | Используется для доступа к базовому объекту **site**

Кроме того, для объектов **driveItem**, к которым предоставлен доступ в личных учетных записях OneDrive, можно использовать указанные ниже связи.

| Имя связи | Тип                         | Описание
| ------------------|:-----------------------------|:-----------------------------------
| **items**         | [**коллекция driveItem**][driveItem] | Все объекты driveItem, содержащиеся в корневой папке, используемой для общего доступа. Перечисление этой коллекции не поддерживается.
| **root**          | [**driveItem**][driveItem]   | Используется для доступа к **основному driveItem**. Обесценилось — используйте `driveItem` вместо этого.

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a>Методы

| Метод                                  | Путь REST                |
| :-------------------------------------- | :----------------------- |
| [Получение общего элемента](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a>Заметки

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->

