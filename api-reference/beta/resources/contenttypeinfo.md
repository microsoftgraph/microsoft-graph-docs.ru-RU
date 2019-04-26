---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: contentTypeInfo
localization_priority: Normal
ms.openlocfilehash: 107dfb3577489521d2e10e0c8fd2fe52c4f90b10
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341231"
---
# <a name="contenttypeinfo-resource-type"></a>Тип ресурса contentTypeInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **contentTypeInfo** указывает тип контента элемента в SharePoint.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **contentTypeInfo** в формате JSON.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a>Свойства

| Имя свойства  | Тип    | Описание
|:---------------|:--------|:--------------------------------------------------
| **id**         | string  | Идентификатор типа контента.
| **name**       | string  | Имя типа контента.

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo",
  "suppressions": []
}
-->
