---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: listInfo
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0e1106873a9f069870c981f6df3ae94412ca85de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987771"
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
