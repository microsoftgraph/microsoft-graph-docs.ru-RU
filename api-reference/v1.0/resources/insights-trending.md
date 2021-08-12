---
title: тип трендовых ресурсов
description: Богатые связи, соединяющие пользователя с документами, которые являются популярными у пользователя (актуальны для пользователя). Файлы OneDrive и файлы, хранящиеся на сайтах групп SharePoint, могут стать актуальными для пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: be87778d9544afc5ec6002ece46ebdb24e3e2c0214ebb5e718885c52bff253fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54216891"
---
# <a name="trending-resource-type"></a>тип трендовых ресурсов

Пространство имен: microsoft.graph

Богатые связи, соединяющие пользователя с документами, которые являются популярными у пользователя (актуальны для пользователя). Файлы OneDrive и файлы, хранящиеся на сайтах групп SharePoint, могут стать актуальными для пользователя.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список "Популярные"](../api/insights-list-trending.md) |Коллекция объектов [trending](insights-trending.md)| Получите список трендовых файлов.|

## <a name="properties"></a>Свойства

| Свойство      | Тип                              | Описание  |
| ------------- |---------------                    | -------------|
| id                    | String                    | Уникальный идентификатор отношения. Только для чтения.        |
| weight                | Двойное с плавающей точкой                    | Значение, указывающее, сколько документа в настоящее время находится в тренде. Чем больше число, тем больше документ в настоящее время находится в тренде вокруг пользователя (чем он актуален). Возвращенные документы сортироваться по этому значению.  |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)    | Свойства, которые можно использовать для визуализации документа в вашем опыте. |
| resourceReference     | [resourceReference](insights-resourcereference.md)        | Справочные свойства документа тренда, например URL-адрес и тип документа. |
| lastModifiedDateTime  | DateTimeOffset            | |
## <a name="relationships"></a>Связи

| Свойство      | Тип          | Описание  |
| ------------- |---------------| -------------|
| resource      | .        | Используется для навигации по документу тренда. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.trending"
}-->

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": {"@odata.type": "microsoft.graph.resourceVisualization"},
  "resourceReference": {"@odata.type": "microsoft.graph.resourceReference"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

