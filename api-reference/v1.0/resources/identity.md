---
author: JeremyKelley
ms.date: 09/10/2017
title: Идентификатор
localization_priority: Normal
description: Ресурс Identity представляет удостоверение субъекта.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b531a4eea8566947c8166f4ab89dd355958c757eb6c768b6504b266c3595a11e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54121265"
---
# <a name="identity-resource-type"></a>Тип ресурса Identity

Пространство имен: microsoft.graph

Ресурс **Identity** представляет удостоверение _субъекта_. В роли субъекта может выступать пользователь, устройство или приложение.

## <a name="json-representation"></a>Описание в формате JSON

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

## <a name="properties"></a>Свойства

| Свойство    | Тип   | Описание                                                                                                                                                                                                                                                                                                           |
|:------------|:-------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| displayName | String | Отображаемое имя удостоверения. Обратите внимание, что оно может не всегда быть доступно или актуально. Например, если пользователь изменит свое отображаемое имя, API может отображать новое значение в последующем ответе, но элементы, сопоставленные с пользователем, будут отображаться без изменения при использовании [разности](../api/driveitem-delta.md).     |
| id          | String | Уникальный идентификатор удостоверения.                                                                                                                                                                                                                                                                                   |

## <a name="remarks"></a>Заметки

В некоторых случаях уникальный идентификатор субъекта может быть недоступен. В таком случае для удостоверения возвращается свойство **displayName**, но в ресурсе будет отсутствовать свойство **id**.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity contains information about an app, user, or group.",
  "keywords": "identity,owner,modifier,app,user,group",
  "section": "documentation",
  "tocPath": "Resources/Identity"

} -->

