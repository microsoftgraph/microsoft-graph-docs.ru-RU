---
title: тенденции тип ресурса
description: Расширенный отношения подключения пользователя к документам, которые прибора вокруг пользователя (являются предназначенных для пользователя). Файлы OneDrive и файлов, хранящихся на сайтах группы SharePoint могут тенденций вокруг пользователя.
author: simonhult
ms.openlocfilehash: ae3c3a876dba6c22a629cce5db8e5b4baa5fb5bf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348001"
---
# <a name="trending-resource-type"></a>тенденции тип ресурса

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Расширенный отношения подключения пользователя к документам, которые прибора вокруг пользователя (являются предназначенных для пользователя). Файлы OneDrive и файлов, хранящихся на сайтах группы SharePoint могут тенденций вокруг пользователя.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список подписок](../api/insights-list-trending.md) |[insights_trending](insights-trending.md) коллекции| Ознакомьтесь со списком тенденции файлы.|

## <a name="properties"></a>Свойства

| Свойство      | Тип                              | Описание  |
| ------------- |---------------                    | -------------|
| id                    | Строка                    | Уникальный идентификатор связи. Только для чтения.        |
| weight                | Double                    | Значение, указывающее, какой объем документ в настоящее время прибора. Чем больше число, тем больше документ — это в настоящее время прибора вокруг пользователя (более качественных это). Возвращенный документы сортируются по это значение.  |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)    | Свойства, которые можно использовать для визуализации документа в работу. |
| resourceReference     | [resourceReference](insights-resourcereference.md)        | Справочник по свойства тенденции документа, например URL-адрес и тип документа. |

## <a name="relationships"></a>Связи

| Свойство      | Тип          | Описание  |
| ------------- |---------------| -------------|
| resource      | Entity        | Используется для перемещения по тенденции документа. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```