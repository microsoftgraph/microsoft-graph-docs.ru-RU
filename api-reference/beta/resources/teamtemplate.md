---
title: Тип ресурса teamTemplate
description: Представляет логический контейнер для всех определений и версий одного и того же шаблона команды.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 489818310abeb39ae4055c7360e8f1d909ea9525
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690169"
---
# <a name="teamtemplate-resource-type"></a>Тип ресурса teamTemplate

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет логический контейнер для всех определений и версий одного и того же шаблона команды.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление teamTemplates](../api/teamwork-list-teamtemplates.md)|[Коллекция teamTemplate](../resources/teamtemplatedefinition.md)| Получение списка объектов **teamTemplate** , доступных для клиента.|
|[Определения списков](../api/teamtemplate-list-definitions.md)| [Коллекция teamTemplateDefinition](../resources/teamtemplatedefinition.md) | Список объектов [teamTemplateDefinition](../resources/teamstemplate.md) , связанных с **teamTemplate**.  |

## <a name="properties"></a>Свойства

| Свойство            | Тип     | Описание |
|:------------------- |:-------- |:----------- |
| id                  | String   | Уникальный идентификатор шаблона. Не может иметь значение NULL. |

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|Определения|[Коллекция teamtemplatedefinition](../resources/teamtemplatedefinition.md)| Универсальное представление определения шаблона команды для команды с определенной структурой и конфигурацией.|

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamtemplate",
}-->

```json
{
  "id": "string"
}
```

## <a name="see-also"></a>См. также

- [team](team.md)
- [teamTemplateDefinition](teamtemplatedefinition.md)
