---
title: тип ресурса usedInsight
description: Представление документов, используемых конкретным пользователем. Сведения возвращают наиболее релевантные документы, которые пользователь просматривал или модифицировал.
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 4163fa241a31b259e87c312b90f07ed05893f682
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036489"
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
| id                    | Строка                    | Уникальный идентификатор отношения. Только для чтения.        |
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

