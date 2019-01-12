---
title: Тип ресурса teamsTemplate
description: Описание сущности teamsTemplate.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9bd5047950ed1ed3c57950d2c4b708a78b570649
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940087"
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

