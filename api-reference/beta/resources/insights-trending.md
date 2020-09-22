---
title: Тип ресурса трендов
description: Отношение с широкими возможностями, соединяющее пользователя с документами, которые обрабатываются пользователем (важны для пользователя). Файлы OneDrive и файлы, хранящиеся на сайтах группы SharePoint, могут обходить пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a083f612b3cb4808a443938a9b7f1958e8c60a0a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986093"
---
# <a name="trending-resource-type"></a>Тип ресурса трендов

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отношение с широкими возможностями, соединяющее пользователя с документами, которые обрабатываются пользователем (важны для пользователя). Файлы OneDrive и файлы, хранящиеся на сайтах группы SharePoint, могут обходить пользователя.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список "Популярные"](../api/insights-list-trending.md) |Коллекция объектов [trending](insights-trending.md)| Получение списка файлов трендов.|

## <a name="properties"></a>Свойства

| Свойство      | Тип                              | Описание  |
| ------------- |---------------                    | -------------|
| id                    | String                    | Уникальный идентификатор связи. Только для чтения.        |
| weight                | Двойное с плавающей точкой                    | Значение, определяющее степень тенденции документа в данный момент. Чем больше это число, тем больше документ будет обходить пользователь (более релевантно). Возвращенные документы сортируются по этому значению.  |
| Ресурсе resourcevisualization | [Ресурсе resourcevisualization](insights-resourcevisualization.md)    | Свойства, которые можно использовать для отображения документа в вашем интерфейсе. |
| ресаурцереференце     | [ресаурцереференце](insights-resourcereference.md)        | Справочные свойства документа тенденций, такие как URL-адрес и тип документа. |
| lastModifiedDateTime  | DateTimeOffset            | |
## <a name="relationships"></a>Связи

| Свойство      | Тип          | Описание  |
| ------------- |---------------| -------------|
| resource      | .        | Используется для навигации по документу трендов. |

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


