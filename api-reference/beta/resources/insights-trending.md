---
title: Тип ресурса трендов
description: Отношение с широкими возможностями, соединяющее пользователя с документами, которые обрабатываются пользователем (важны для пользователя). Файлы OneDrive и файлы, хранящиеся на сайтах группы SharePoint, могут обходить пользователя.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 7963a3c518fd4fc946da4f6714a3aa52aa4b87eb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006222"
---
# <a name="trending-resource-type"></a>Тип ресурса трендов

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отношение с широкими возможностями, соединяющее пользователя с документами, которые обрабатываются пользователем (важны для пользователя). Файлы OneDrive и файлы, хранящиеся на сайтах группы SharePoint, могут обходить пользователя.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список "Популярные"](../api/insights-list-trending.md) |Коллекция [инсигхтс_трендинг](insights-trending.md)| Получение списка файлов трендов.|

## <a name="properties"></a>Свойства

| Свойство      | Тип                              | Описание  |
| ------------- |---------------                    | -------------|
| id                    | String                    | Уникальный идентификатор связи. Только для чтения.        |
| weight                | Двойное                    | Значение, определяющее степень тенденции документа в данный момент. Чем больше это число, тем больше документ будет обходить пользователь (более релевантно). Возвращенные документы сортируются по этому значению.  |
| Ресурсе resourcevisualization | [Ресурсе resourcevisualization](insights-resourcevisualization.md)    | Свойства, которые можно использовать для отображения документа в вашем интерфейсе. |
| Ресаурцереференце     | [Ресаурцереференце](insights-resourcereference.md)        | Справочные свойства документа тенденций, такие как URL-адрес и тип документа. |
| lastModifiedDateTime  | DateTimeOffset            | |
## <a name="relationships"></a>Отношения

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
