---
author: JeremyKelley
title: Тип ресурса identity
ms.localizationpriority: medium
description: Представляет удостоверение субъекта.
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 5a266b1a3dab7a1f9de23e296c38336f25e86dd0
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856276"
---
# <a name="identity-resource-type"></a>Тип ресурса identity

Пространство имен: microsoft.graph

Представляет удостоверение _субъекта_. В роли субъекта может выступать пользователь, устройство или приложение.

В некоторых случаях уникальный идентификатор субъекта может быть недоступен.
В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                                                                                                                                                                                                                                                                                                           |
|:------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| displayName | Строка | Отображаемое имя удостоверения. Обратите внимание, что это может быть не всегда доступно или актуально. Например, если пользователь изменяет отображаемое имя, API может отобразить новое значение в следующем ответе, но элементы, связанные с пользователем, не будут отображаться как измененные при использовании [delta.](../api/driveitem-delta.md)     |
| id          | String | Уникальный идентификатор удостоверения.                                                                                                                                                                                                                                                                                   |

## <a name="json-representation"></a>Представление JSON

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identity",
  "openType": true,
 "optionalProperties": ["displayName", "thumbnails"] } -->
```json
{
  "displayName": "string",
  "id": "string",
  "thumbnails": { "@odata.type": "microsoft.graph.thumbnailSet" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity"

} -->

