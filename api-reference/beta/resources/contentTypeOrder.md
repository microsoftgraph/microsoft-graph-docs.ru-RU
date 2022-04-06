---
author: daspek
description: Ресурс contentTypeOrder указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.
ms.date: 09/13/2017
title: contentTypeOrder
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 615655ecf400c814e08ef75dfbabd9a5f97cf167
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63720832"
---
# <a name="contenttypeorder-resource-type"></a>Тип ресурса contentTypeOrder

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **contentTypeOrder** указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **contentTypeOrder** в формате JSON.

<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a>Свойства

| Свойство     | Тип    | Описание                                                                   |
| :----------- | :------ | :---------------------------------------------------------------------------- |
| **default**  | boolean | Указывает, используется ли этот тип контента по умолчанию.                                      |
| **position** | Int32   | Указывает позицию, в которой тип контента отображается в пользовательском интерфейсе выбора. |

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder",
  "suppressions": []
}
-->
