---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: contentTypeOrder
ms.openlocfilehash: a6b83627d86bbb35357f03dbee3605c6fb1df7a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081784"
---
# <a name="contenttypeorder-resource-type"></a>Тип ресурса contentTypeOrder

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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

| Имя свойства | Тип    | Описание
|:--------------|:--------|:----------------------------------------------------
| **default**   | логический | Указывает, используется ли этот тип контента по умолчанию.
| **position**  | Int32   | Указывает позицию, в которой тип контента отображается в пользовательском интерфейсе выбора.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
