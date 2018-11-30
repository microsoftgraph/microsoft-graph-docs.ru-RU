---
title: тенденции тип ресурса
description: Расширенный отношения подключения пользователя к документам, которые прибора вокруг пользователя (являются предназначенных для пользователя). Файлы OneDrive и файлов, хранящихся на сайтах группы SharePoint могут тенденций вокруг пользователя.
ms.openlocfilehash: 7d240c4358047ca9ba3d6b8340fbfb7d893a6a1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078829"
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
| id                    | String                    | Уникальный идентификатор связи. Только для чтения.        |
| weight                | Double                    | Значение, указывающее, какой объем документ в настоящее время прибора. Чем больше число, тем больше документ — это в настоящее время прибора вокруг пользователя (более качественных это). Возвращенный документы сортируются по это значение.  |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)    | Свойства, которые можно использовать для визуализации документа в работу. |
| resourceReference     | [resourceReference](insights-resourcereference.md)        | Справочник по свойства тенденции документа, например URL-адрес и тип документа. |

## <a name="relationships"></a>Связи

| Свойство      | Тип          | Описание  |
| ------------- |---------------| -------------|
| resource      | Объект        | Используется для перемещения по тенденции документа. |

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