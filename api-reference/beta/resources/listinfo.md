---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: listInfo
localization_priority: Normal
ms.openlocfilehash: c1a29099264c46f32e09b375a97ff49c13c99c6f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858459"
---
# <a name="listinfo-resource"></a>Ресурс listInfo

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Сложный тип **listInfo** используется для хранения дополнительных сведений о [списке][].

[list]: list.md

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.listInfo"
}-->

```json
{
  "contentTypesEnabled": false,
  "hidden": false,
  "template": "documentLibrary | genericList | tasks | survey | links | announcements | contacts | ..."
}
```

## <a name="properties"></a>Свойства

| Имя свойства           | Тип    | Описание
|:------------------------|:--------|:------------------------------------------------
| **contentTypesEnabled** | Boolean | Если свойство имеет значение `true`, это указывает на то, что для этого списка разрешено использовать типы контента.
| **hidden**              | Boolean | Если это свойство имеет значение `true`, это указывает на то, что список обычно не отображается в пользовательском интерфейсе SharePoint.
| **template**            | String  | Перечислимое значение, которое представляет базовый шаблон списка, используемый при создании списка. Возможные значения: `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts` и другие.

### <a name="remarks"></a>Примечания

Большинство списков, создаваемых пользователями, будут иметь одно из указанных выше значений, но можно также использовать и другие значения.
Ваше приложение должно быть способно обрабатывать любые значения, которые не указаны здесь.
Для разработчиков, знакомых с API CSOM в SharePoint, значение `template` соответствует перечислению `SPListTemplateType`.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
