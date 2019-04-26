---
title: Тип ресурса insights
description: Аналитика — это связи, вычисленные с помощью расширенного анализа и методов машинного обучения. К примеру, вы можете выявить документы OneDrive, пользующиеся популярностью у пользователей.
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 4e71dbca7bf4ebbe054d0da83436e5dc2129cf19
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551899"
---
# <a name="insights-resource-type"></a>Тип ресурса insights

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Аналитика — это связи, вычисленные с помощью расширенного анализа и методов машинного обучения. К примеру, вы можете выявить документы OneDrive, пользующиеся популярностью у пользователей.

Аналитика возвращается с помощью указанных ниже API.

- [Популярные](insights-trending.md) — возвращает документы из OneDrive и сайтов SharePoint, популярные у пользователя.
- [Использованные](insights-used.md) — возвращает документы, просмотренные и измененные пользователем. Включает документы, используемые пользователем в OneDrive для бизнеса, SharePoint, открытые как вложения почты и вложенные ссылки из таких источников, как Box, DropBox и Google Диск.
- [Общие](insights-shared.md) — возвращает документы, к которым пользователю предоставлен общий доступ. Документы могут предоставляться в виде вложений электронной почты или ссылок OneDrive для бизнеса, отправленных в сообщениях электронной почты.

Каждый объект аналитики возвращается со значением сложного типа (CVT) `resourceVisualization` и `resourceReference`. Значение CVT resourceVisualization содержит свойства, например `title` и `previewImageUrl`. Корпорация Майкрософт использует свойства визуализации для отображения файлов в интерфейсах, таких как Office Delve.

## <a name="relationships"></a>Связи

| Отношение      | Тип          | Описание  |
| ------------- |---------------| -------------|
| trending      | Коллекция [Trending](insights-trending.md)       | Вычисляемая связь, определяющая популярные документы. Популярные документы могут храниться в OneDrive или на сайтах SharePoint.   |
| used      | Коллекция [Used](insights-used.md)       | Вычисляемая связь, определяющая документы, просмотренные и измененные пользователем. Включает документы, используемые пользователем в OneDrive для бизнеса, SharePoint, открытые как вложения почты и вложенные ссылки из таких источников, как Box, DropBox и Google Диск.  |
| shared        | Коллекция [Shared](insights-shared.md)       | Вычисляемая связь, определяющая документы, к которым пользователю предоставлен общий доступ. Документы могут предоставляться в виде вложений электронной почты или ссылок OneDrive для бизнеса, отправленных в сообщениях электронной почты.   |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.
```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
