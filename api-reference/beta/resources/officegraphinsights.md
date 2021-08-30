---
title: Тип ресурса officeGraphInsights
description: Представляет базовый тип для itemInsights. officeGraphInsights предназначен для обратной совместимости с более ранними версиями API аналитики. Используйте только itemInsights при получении доступа к API аналитики.
author: simonhult
ms.localizationpriority: high
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 308d35e19eaf1ac5454b33b030d2e9c0a7f7a416
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695919"
---
# <a name="officegraphinsights-resource-type"></a>Тип ресурса officeGraphInsights

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте [itemInsights](iteminsights.md) вместо **officeGraphInsights**, чтобы получить доступ к API аналитики.

**officeGraphInsights** предназначен для обратной совместимости с более ранними версиями API аналитики. Это базовый тип для [itemInsights](iteminsights.md).

Аналитика — это связи, вычисленные с помощью расширенного анализа и методов машинного обучения. К примеру, вы можете выявить документы OneDrive для бизнеса, пользующиеся популярностью у пользователей.

Аналитика возвращается с помощью указанных ниже API.

- [Популярные](insights-trending.md) — возвращает документы из OneDrive для бизнеса и сайтов SharePoint, популярные у пользователя.
- [Использованные](insights-used.md) — возвращает документы, просмотренные и измененные пользователем. Включает документы, использованные пользователем в OneDrive для бизнеса и SharePoint.
- [Общие](insights-shared.md) — возвращает документы, к которым пользователю или пользователем предоставлен общий доступ. Общий доступ к документам можно предоставлять в виде по URL-ссылок, вложенных файлов, справочных вложений в OneDrive для бизнеса и файлам SharePoint, которые есть в сообщениях и собраниях Outlook.

Каждый объект аналитики возвращается со значением сложного типа (CVT) **resourceVisualization** и **resourceReference** сложного типа значений. Сложный тип значений **resourceVisualization** содержит такие свойства, как **title** и **previewImageUrl**. Корпорация Майкрософт использует свойства визуализации для отображения файлов в интерфейсах, таких как Office Delve.

## <a name="relationships"></a>Связи

| Связь      | Тип          | Описание  |
| ------------- |---------------| -------------|
| trending      | Коллекция объектов [trending](insights-trending.md)       | Получите доступ к этому свойству из производного типа [itemInsights](iteminsights.md).|
| used      | Коллекция объектов [usedInsight](insights-used.md)        | Получите доступ к этому свойству из производного типа [itemInsights](iteminsights.md).|
| общие        | Коллекция объектов [sharedInsight](insights-shared.md)        | Получите доступ к этому свойству из производного типа [itemInsights](iteminsights.md).|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "baseType":"microsoft.graph.entity",
  "optionalProperties": [
    "trending",
    "used",
    "shared"
  ],
  "@odata.type": "microsoft.graph.officeGraphInsights"
}-->

```json
{
  "id": "string",
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```



