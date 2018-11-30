---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: contentTypeInfo
ms.openlocfilehash: 922f87c77280627efb956e4558e1ff269daa9311
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079125"
---
# <a name="contenttypeinfo-resource-type"></a>Тип ресурса contentTypeInfo

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
| **id**         | строка  | Идентификатор типа контента.
| **name**       | строка  | Имя типа контента.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo"
} -->
