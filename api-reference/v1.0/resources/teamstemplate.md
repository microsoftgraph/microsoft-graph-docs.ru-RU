---
title: teamsTemplate resource type
description: Описывает объект teamsTemplate.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5adcd554c687747fb45cdfd1a40e9e37cfaad2d9107a43ebc2ceca01b5d94f3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249127"
---
# <a name="teamstemplate-resource-type"></a>teamsTemplate resource type

Пространство имен: microsoft.graph

Шаблон группы — это план [](../resources/team.md) создания группы в Microsoft Teams. Шаблон указывает структуру, параметры и даже содержимое, которое должно быть разработано в новой группе, созданной с помощью шаблона. Корпорация Майкрософт предоставляет набор базовых шаблонов, и клиенты могут сохранять собственные пользовательские шаблоны.

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | String   | Уникальный идентификатор шаблона. Не может быть null. |

## <a name="json-representation"></a>Представление в формате JSON

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

## <a name="see-also"></a>См. также

- [team](team.md)


