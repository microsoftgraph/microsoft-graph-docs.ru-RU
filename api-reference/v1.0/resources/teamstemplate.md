---
title: teamsTemplate resource type
description: Описывает объект teamsTemplate.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3ef812716b2650e7919d18291f1f43c9adf878b5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098414"
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


