---
title: Тип ресурса recentNotebook
description: Недавно открытая записная книжка OneNote. Ресурс **recentNotebook** похож на ресурс notebook, но имеет меньше свойств.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 948d3deed4e2bc51e95f0e04b5e962b09eb69195
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965511"
---
# <a name="recentnotebook-resource-type"></a>Тип ресурса recentNotebook

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Недавно открытая записная книжка OneNote. Ресурс **recentNotebook** похож на ресурс [notebook](notebook.md), но имеет меньше свойств.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|String|Имя записной книжки.|
|lastAccessedTime|DateTimeOffset|Дата и время последнего изменения записной книжки. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения.|
|links|[recentNotebookLinks](recentnotebooklinks.md)|Ссылки для открытия записной книжки. Ссылка `oneNoteClientURL` открывает записную книжку в клиенте OneNote, если он установлен. `oneNoteWebURL` Ссылка открывает записную книжку в OneNote в Интернете.|
|sourceService|String|Внутреннее хранилище, в котором находится записная книжка (`OneDriveForBusiness` или `OneDrive`).|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebook"
}-->

```json
{
  "displayName": "String",
  "lastAccessedTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.recentNotebookLinks"},
  "sourceService": "String"
}

```

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[getRecentNotebooks](../api/notebook-getrecentnotebooks.md) | Коллекция [notebook](notebook.md) | Получите коллекцию записных книжек, которые недавно открывал пользователь. |
