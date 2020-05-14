---
title: Тип ресурса Усединсигхт
description: Представление документов, используемых определенным пользователем. Аналитика возвращает наиболее релевантные документы, которые пользователь просматривал или изменил.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: aa5d5adc9b7716f26c1b05edb00122da57d625ab
ms.sourcegitcommit: a21fa7fad3a75f94e924b36d6ab94a3699983bdf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/14/2020
ms.locfileid: "44227019"
---
# <a name="usedinsight-resource-type"></a>Тип ресурса Усединсигхт

Пространство имен: microsoft.graph

Представление документов, используемых определенным пользователем. Аналитика возвращает наиболее релевантные документы, которые пользователь просматривал или изменил. Сюда входят документы в:

- OneDrive для бизнеса
- SharePoint

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список "Использованные"](../api/insights-list-used.md) |Коллекция объектов [usedInsight](insights-used.md)| Получение списка используемых файлов.|

## <a name="properties"></a>Свойства

| Свойство              | Тип                      | Описание  |
| -------------         |---------------            | -------------|
| id                    | String                    | Уникальный идентификатор связи. Только для чтения.        |
| ластусед              | [usageDetails](insights-usagedetails.md)              | Сведения о том, когда элемент был последний раз просмотрен или изменен пользователем. Только для чтения.      |
| Ресурсе resourcevisualization | [Ресурсе resourcevisualization](insights-resourcevisualization.md)                | Свойства, которые можно использовать для отображения документа в вашем интерфейсе. Только для чтения      |
| ресаурцереференце     | [ресаурцереференце](insights-resourcereference.md)                      | Справочные свойства используемого документа, например URL-адрес и тип документа. Только для чтения     |

## <a name="relationships"></a>Связи

| Свойство      | Тип          | Описание  |
| ------------- |---------------| -------------|
| resource      | Коллекция [объектов](entity.md)    | Используется для перехода к использованному элементу. Для вложений в файл используется тип *fileAttachment*. Для связанных вложений используется тип *driveItem*. |

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
