---
author: JeremyKelley
title: Тип ресурса sharedDriveItem
ms.localizationpriority: medium
description: Ресурс sharedDriveItem возвращается при использовании API общих ресурсов для доступа к общему объекту driveItem.
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 52fa1c8d4395283f6e33464142eab0f411fd46ac
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034588"
---
# <a name="shareddriveitem-resource-type"></a>Тип ресурса sharedDriveItem

Пространство имен: microsoft.graph

Ресурс **sharedDriveItem** возвращается при [использовании API](../api/shares-get.md) общих ресурсов для доступа к [общему объекту driveItem](driveitem.md).

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
| owner    | [identitySet](identityset.md) | Сведения о владельце общего элемента, ставшего объектом ссылки. |

## <a name="relationships"></a>Связи

| Имя связи | Тип                | Описание
| ------------------|:--------------------|:-----------------------------------
| **driveItem**     | [**driveItem**][driveItem]   | Используется для доступа к базовому объекту **driveItem**
| **list**          | [**list**][list]        | Используется для доступа к базовому объекту **list**
| **listItem**      | [**listItem**][listItem]    | Используется для доступа к базовому объекту **listItem**
| **permission**    | [**Разрешение**][permission] | Используется для доступа к **разрешению,** представляющего базовую ссылку для общего доступа.
| **site**          | [**site**][site]        | Используется для доступа к базовому объекту **site**

Кроме того, для объектов **driveItem**, к которым предоставлен доступ в личных учетных записях OneDrive, можно использовать указанные ниже связи.

| Имя связи | Тип                         | Описание
| ------------------|:-----------------------------|:-----------------------------------
| **items**         | [**Коллекция driveItem**][driveItem] | Все объекты driveItem, содержащиеся в корневой папке, используемой для общего доступа. Перечисление этой коллекции не поддерживается.
| **root**          | [**driveItem**][driveItem]   | Используется для доступа к базовому **объекту driveItem**. Нерекомендуемый — используйте `driveItem` вместо него.

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

Дополнительные сведения о аспектах в DriveItem см. [в разделе driveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->

