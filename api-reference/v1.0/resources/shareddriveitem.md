---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
ms.openlocfilehash: 0d0c5a34d12fe467196c0616befc7376835b632c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481729"
---
# <a name="shareddriveitem-resource-type"></a>Тип ресурса SharedDriveItem

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
| id       | String                        | Уникальный идентификатор для общего ресурса, к которому предоставляется доступ.              |
| name     | Строка                        | Отображаемое имя общего элемента.                             |
| owner    | [IdentitySet](identityset.md) | Сведения о владельце общего элемента, ставшего объектом ссылки. |

## <a name="relationships"></a>Связи

| Имя связи | Тип                | Описание
| ------------------|:--------------------|:-----------------------------------
| **driveItem**     | [**driveItem**][driveItem]   | Используется для доступа к базовому объекту **driveItem**
| **list**          | [**list**][list]        | Используется для доступа к базовому объекту **list**
| **listItem**      | [**listItem**][listItem]    | Используется для доступа к базовому объекту **listItem**
| **site**          | [**site**][site]        | Используется для доступа к базовому объекту **site**

Кроме того, для объектов **driveItem**, к которым предоставлен доступ в личных учетных записях OneDrive, можно использовать указанные ниже связи.

| Имя связи | Тип                         | Описание
| ------------------|:-----------------------------|:-----------------------------------
| **items**         | Коллекция объектов [**driveItem**][driveItem] | Все объекты driveItem, содержащиеся в корневой папке, используемой для общего доступа. Перечисление этой коллекции не поддерживается.
| **root**          | [**driveItem**][driveItem]   | Используется для доступа к базовому **driveItem**. Рекомендуется использовать `driveItem` вместо этого.

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
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
