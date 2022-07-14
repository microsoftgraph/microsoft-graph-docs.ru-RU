---
title: Тип ресурса searchSettings
description: Собирает все настраиваемые параметры, связанные с поиском по содержимому соединителя.
author: emzho
ms.localizationpriority: normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f0915d57f0c49199f0273b8c44d5f60b2d78531c
ms.sourcegitcommit: 033e779ba738b61b03e2760f39554a2fd0ab65b4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2022
ms.locfileid: "66788635"
---
# <a name="searchsettings-resource-type"></a>Тип ресурса searchSettings

Пространство имен: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Собирает все настраиваемые параметры, связанные с поиском по содержимому соединителя.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|searchResultTemplates|[Коллекция microsoft.graph.externalConnectors.displayTemplate](../resources/externalconnectors-displaytemplate.md)|Позволяет разработчику определить внешний вид содержимого и настроить условия, определяющие, когда должен отображаться шаблон. Не более 2 шаблонов результатов поиска на подключение.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.searchSettings"
}
-->
``` json
{
  "searchResultTemplates": [
    {
      "id": "String (identifier)",
      "rules": [
        {
          "property": "itemTitle",
          "operation": "contains",
          "valuesJoinedBy": "or",
          "values": [
              "contoso",
              "smart"
          ]
        }
      ],
      "layout": {"type": "AdaptiveCard","version": "1.0","body": [{"type": "TextBlock","text": "A contoso ticket."}]},
      "priority": 0
    },
        {
      "id": "String (identifier)",
      "rules": [
        {
          "property": "itemDescription",
          "operation": "contains",
          "valuesJoinedBy": "and",
          "values": [
              "contoso",
              "ticket"
          ]
        }
      ],
      "layout": {"type": "AdaptiveCard","version": "1.0","body": [{"type": "TextBlock","text": "A contoso ticket."}]},
      "priority": 1
    }
  ]
}
```

