---
title: тип ресурса usedInsight
description: Представление документов, используемых конкретным пользователем. Сведения возвращают наиболее релевантные документы, которые пользователь просматривал или модифицировал.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 6c1933231c9294daf4cccfeeba41ecd71582e3fe4324e28121f40b444c848e34
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230692"
---
# <a name="usedinsight-resource-type"></a>тип ресурса usedInsight

Пространство имен: microsoft.graph

Представление документов, используемых конкретным пользователем. Сведения возвращают наиболее релевантные документы, которые пользователь просматривал или модифицировал. Это включает в себя документы в:

- OneDrive для бизнеса
- SharePoint

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список "Использованные"](../api/insights-list-used.md) |Коллекция объектов [usedInsight](insights-used.md)| Получите список используемых файлов.|

## <a name="properties"></a>Свойства

| Свойство              | Тип                      | Описание  |
| -------------         |---------------            | -------------|
| id                    | String                    | Уникальный идентификатор отношения. Только для чтения.        |
| lastUsed              | [usageDetails](insights-usagedetails.md)              | Сведения о том, когда элемент был в последний раз просмотрен или изменен пользователем. Только для чтения.      |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | Свойства, которые можно использовать для визуализации документа в вашем опыте. Только для чтения      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Справочные свойства используемого документа, например URL-адрес и тип документа. Только для чтения     |

## <a name="relationships"></a>Связи

| Свойство      | Тип          | Описание  |
| ------------- |---------------| -------------|
| resource      | [Коллекция сущности](entity.md)    | Используется для навигации по элементу, который был использован. Для вложений файлов тип *fileAttachment*. Для связанных вложений тип *driveItem*. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "resource"
  ],
  "@odata.type": "microsoft.graph.usedInsight"
}-->

```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": { "@odata.type": "microsoft.graph.resourceVisualization" },
  "resourceReference": { "@odata.type": "microsoft.graph.resourceReference" }
}
```

