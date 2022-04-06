---
author: JeremyKelley
description: Сложный тип listInfo используется для хранения дополнительных сведений о списке.
ms.date: 09/11/2017
title: ListInfo
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a2174c4fda353d0bfa5148f8ec5985f925ff0070
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63723806"
---
# <a name="listinfo-resource"></a>Ресурс listInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип **listInfo** используется для хранения дополнительных сведений о [списке][].

[списке]: list.md

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type&quot;: &quot;microsoft.graph.listInfo"
}-->

```json
{
  "contentTypesEnabled": false,
  "hidden": false,
  "template&quot;: &quot;documentLibrary | genericList | tasks | survey | links | announcements | contacts | ..."
}
```

## <a name="properties"></a>Свойства

| Свойство                | Тип    | Описание                                                                                                                                                                                              |
| :---------------------- | :------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **contentTypesEnabled** | Boolean | Если свойство имеет значение `true`, это указывает на то, что для этого списка разрешено использовать типы контента.                                                                                                                                       |
| **hidden**              | Boolean | Если это свойство имеет значение `true`, это указывает на то, что список обычно не отображается в пользовательском интерфейсе SharePoint.                                                                                                            |
| **template**            | String  | Перечислимое значение, которое представляет базовый шаблон списка, используемый при создании списка. Возможные значения: `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` и другие. |

### <a name="remarks"></a>Замечания

Большинство списков, создаваемых пользователями, будут иметь одно из указанных выше значений, но можно также использовать и другие значения.
Ваше приложение должно быть способно обрабатывать любые значения, которые не указаны здесь.
Для разработчиков, знакомых с API CSOM в SharePoint, значение `template` соответствует перечислению `SPListTemplateType`.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
