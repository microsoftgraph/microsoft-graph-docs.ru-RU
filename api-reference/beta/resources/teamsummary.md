---
title: тип ресурса teamSummary
description: Содержит сведения о команде в Microsoft Teams, включая число владельцев, членов и гостей.
ms.localizationpriority: medium
author: akhilkohlimicrosoft
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 497ac22cf95c30b4510c08b04e591c7acaf8c449
ms.sourcegitcommit: 0fa7148e0b776663eaca3e79e72b85046d4b8b1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/15/2022
ms.locfileid: "63500985"
---
# <a name="teamsummary-resource-type"></a>тип ресурса teamSummary

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о команде в Microsoft Teams, включая количество владельцев, членов и гостей.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|guestsCount|Int32|Количество гостей в команде.|
|membersCount|Int32|Количество участников в команде.|
|ownersCount|Int32|Количество владельцев в команде.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamSummary"
}-->

```json
{
    "guestsCount": "Integer",
    "membersCount": "Integer",
    "ownersCount": "Integer",
}
```


