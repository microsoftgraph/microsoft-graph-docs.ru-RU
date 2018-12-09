---
title: Тип ресурса teamsTemplate
description: Описание сущности teamsTemplate.
ms.openlocfilehash: 76b2921e884d38a57097789b1ba64df3309d141c
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2018
ms.locfileid: "27210161"
---
# <a name="teamstemplate-resource-type"></a>Тип ресурса teamsTemplate

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Шаблон группы — это план для создания [группы](../resources/team.md) в группами Майкрософт. Шаблон указывает структуры, параметры и даже контента, который следует предоставить в новые группы, созданные на основе шаблона. Корпорация Майкрософт предоставляет набор базовых шаблонов и пользователи могут сохранять свои собственные пользовательские шаблоны.

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | Строка   | Уникальный идентификатор шаблона. Не может быть null. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a>См. также

- [Группа](team.md)

