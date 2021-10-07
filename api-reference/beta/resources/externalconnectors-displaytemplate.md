---
title: тип ресурса displayTemplate
description: Определяет внешний вид контента и условия, которые диктуют, когда должен отображаться шаблон.
author: emzho
ms.localizationpriority: normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5138bb43bea3aec216dcb86ffc2f09eaec96e315
ms.sourcegitcommit: 2a9b82dae63d8a998711679a379ae1fa89df80e0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/06/2021
ms.locfileid: "60214949"
---
# <a name="displaytemplate-resource-type"></a>тип ресурса displayTemplate

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет внешний вид контента и условия, которые диктуют, когда должен отображаться шаблон.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор текста для шаблона отображения; например, `contosoTickets` .|
|макет|[microsoft.graph.Json](../resources/intune-mam-json.md)|Определение внешнего вида контента, представленное адаптивной картой [,](https://docs.microsoft.com/adaptive-cards/authoring-cards/getting-started)которая представляет собой объектную модель объекта JSON-serialized.|
|priority|Int32|Определяет приоритет шаблона отображения. Шаблон отображения с приоритетом 1 оценивается перед шаблоном с приоритетом 4. Поддерживаются пробелы в значениях приоритетов.|
|правила|[коллекция microsoft.graph.externalConnectors.propertyRule](../resources/externalconnectors-propertyrule.md)|Указывает дополнительные правила выбора этого шаблона отображения на основе схемы элемента. Необязательный параметр.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.displayTemplate"
}
-->
``` json
    {
      "id": "String",
      "rules": [
        {
          "property": "String",
          "operation": "String",
          "valuesJoinedBy": "String",
          "values": [
              "String",
              "String"
          ]
        }
      ],
      "layout": {"type": "AdaptiveCard","version": "1.0","body": [{"type": "TextBlock","text": "String"}]},
      "priority": 0
    }
```

