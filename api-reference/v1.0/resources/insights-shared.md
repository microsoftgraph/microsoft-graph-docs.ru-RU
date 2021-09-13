---
title: тип ресурса sharedInsight
description: 'Представление, представляющее файлы, общие конкретному пользователю или его пользователю. Поддерживаются следующие общие файлы:'
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3e9762c2da54f10e28e0337930972c6a6094ac65
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118588"
---
# <a name="sharedinsight-resource-type"></a>тип ресурса sharedInsight

Пространство имен: microsoft.graph

Представление, представляющее файлы, общие конкретному пользователю или его пользователю. Поддерживаются следующие общие файлы:

- Файлы, присоединенные непосредственно к электронной почте или приглашению на собрание.
- OneDrive для бизнеса и SharePoint вложения — файлы, хранимые в OneDrive для бизнеса и SharePoint, которые пользователи делятся как ссылки в электронной почте.

**Примечание.** В настоящее время мы работаем над заполнением результатов общего API данными. Некоторые данные могут быть пропущены в первые недели после выпуска.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список "Общие"](../api/insights-list-shared.md) |Коллекция объектов [sharedInsight](insights-shared.md)| Получите список общих файлов.|

## <a name="properties"></a>Свойства

| Свойство              | Тип                      | Описание  |
| -------------         |---------------            | -------------|
| id                    | Строка                    | Уникальный идентификатор отношения. Только для чтения.        |
| lastShared            | [sharingDetail](insights-sharingdetail.md)                | Сведения об общем элементе. Только для чтения.        |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | Свойства, которые можно использовать для визуализации документа в вашем опыте. Только для чтения      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Справочные свойства общего документа, например URL-адрес и тип документа. Только для чтения       |

## <a name="relationships"></a>Отношения

| Свойство      | Тип          | Описание  |
| ------------- |---------------| -------------|
| resource      | Коллекция сущности | Используется для навигации по элементу, который был общим. Для вложений файлов тип *fileAttachment*. Для связанных вложений тип *driveItem*. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType":"resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedInsight"
}-->
```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```

