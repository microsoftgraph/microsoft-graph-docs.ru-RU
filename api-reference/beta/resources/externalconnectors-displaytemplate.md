---
title: Тип ресурса displayTemplate
description: Определяет внешний вид содержимого и условия, определяющие, когда должен отображаться шаблон.
author: emzho
ms.localizationpriority: normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a20b9935ad142fce0a1b1fcd2a47e608a0fec670
ms.sourcegitcommit: 033e779ba738b61b03e2760f39554a2fd0ab65b4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2022
ms.locfileid: "66788768"
---
# <a name="displaytemplate-resource-type"></a>Тип ресурса displayTemplate

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Определяет внешний вид содержимого и условия, определяющие, когда должен отображаться шаблон.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Текстовый идентификатор шаблона отображения; Например, `contosoTickets`. Не более 16 символов. Разрешены только буквенно-цифровые символы. |
|Макет|[microsoft.graph.Json](../resources/intune-mam-json.md)|Определение внешнего вида содержимого, представленное адаптивной карточкой [, которая](/adaptive-cards/authoring-cards/getting-started) представляет собой сериализованную в формате JSON объектную модель карточки.|
|priority|Int32|Определяет приоритет шаблона отображения. Шаблон отображения с приоритетом 1 оценивается перед шаблоном с приоритетом 4. Поддерживаются пробелы в значениях приоритета. Должно быть положительным значением.|
|правила|[Коллекция microsoft.graph.externalConnectors.propertyRule](../resources/externalconnectors-propertyrule.md)|Задает дополнительные правила выбора этого шаблона отображения на основе схемы элемента. Необязательный элемент.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
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