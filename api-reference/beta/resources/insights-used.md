---
title: используемый тип ресурса
description: Возможность получения, представляющее документы, используемые для определенного пользователя. Возвращает полезные сведения о наиболее важные документы, которые пользователь просматривать или доступны.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 2f8479896f8c06fdc6193cfa8c18a0c3d8293bc7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976061"
---
# <a name="used-resource-type"></a>используемый тип ресурса

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Возможность получения, представляющее документы, используемые для определенного пользователя. Возвращает полезные сведения о наиболее важные документы, которые пользователь просматривать или доступны. Документы в том числе:

- OneDrive для бизнеса
- SharePoint

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список, используемый](../api/insights-list-used.md) |[insights_used](insights-used.md) коллекции| Ознакомьтесь со списком используемые файлы.|

## <a name="properties"></a>Свойства

| Свойство              | Тип                      | Описание  |
| -------------         |---------------            | -------------|
| id                    | String                    | Уникальный идентификатор связи. Только для чтения.        |
| lastUsed              | [usageDetails](insights-usagedetails.md)              | Сведения о последнего элемента просматривать и изменять пользователем. Только для чтения.     |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | Свойства, которые можно использовать для визуализации документа в работу. Только для чтения      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Справочник по свойства используется документа, например URL-адрес и тип документа. Только для чтения     |

## <a name="relationships"></a>Связи

| Свойство      | Тип          | Описание  |
| ------------- |---------------| -------------|
| resource      | Entity        | Используется для перехода к элементу, который использовался. Для файлов вложений тип — *fileAttachment*. Для связанного вложения тип — *driveItem*. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
