---
author: JeremyKelley
description: Сложный тип listInfo используется для хранения дополнительных сведений о списке.
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5f36e7f08d8a5ce29316e97ff8f03f14063a4d36
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055290"
---
# <a name="listinfo-resource"></a>Ресурс listInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип **listInfo** используется для хранения дополнительных сведений о [списке][].

[списке]: list.md

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


