---
title: Тип ресурса teamsTemplate
description: Описывает сущность teamsTemplate.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d20d759476177541ed51ff40edec6188290cbbb1
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690023"
---
# <a name="teamstemplate-resource-type"></a>Тип ресурса teamsTemplate

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Шаблон команды — это схема для создания [команды](../resources/team.md) в Microsoft Teams. Шаблон указывает структуру, параметры и даже содержимое, которое должно быть подготовлено в новой команде, созданной с помощью шаблона. Корпорация Майкрософт предоставляет набор базовых шаблонов, и клиенты могут сохранять собственные настраиваемые шаблоны.

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | Строка   | Уникальный идентификатор шаблона. Не может иметь значение NULL. |

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
- [teamTemplateDefinition](teamtemplatedefinition.md)



