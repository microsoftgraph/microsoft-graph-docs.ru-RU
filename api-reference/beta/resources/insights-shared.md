---
title: Тип ресурса Шарединсигхт
description: 'Понимание файлов, к которым предоставлен общий доступ, или определенного пользователя. Поддерживаются следующие общие файлы:'
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 128a85bb9aa2e9f51d2393029cce3c27f8c4e6f8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339998"
---
# <a name="sharedinsight-resource-type"></a>Тип ресурса Шарединсигхт

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Понимание файлов, к которым предоставлен общий доступ, или определенного пользователя. Поддерживаются следующие общие файлы:

- Файлы, вложенные непосредственно в сообщение электронной почты или приглашение на собрание.
- OneDrive для Буссинесс и современных вложений SharePoint — файлы, хранящиеся в OneDrive для бизнеса и SharePoint, которые пользователи совместно используют как ссылки в сообщениях электронной почты.

**Note**: в настоящее время мы работаем над заполнением результатов общего API с данными. Некоторые данные могут отсутствовать в первых неделях после выпуска.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список "Общие"](../api/insights-list-shared.md) |Коллекция [инсигхтс_шаред](insights-shared.md)| Получение списка общих файлов.|

## <a name="properties"></a>Свойства

| Свойство              | Тип                      | Описание  |
| -------------         |---------------            | -------------|
| id                    | String                    | Уникальный идентификатор связи. Только для чтения.        |
| Ластшаред            | [sharingDetail](insights-sharingdetail.md)                | Сведения об общем элементе. Только для чтения.        |
| Ресурсе resourcevisualization | [Ресурсе resourcevisualization](insights-resourcevisualization.md)                | Свойства, которые можно использовать для отображения документа в вашем интерфейсе. Только для чтения      |
| Ресаурцереференце     | [Ресаурцереференце](insights-resourcereference.md)                      | Справочные свойства общего документа, например URL-адрес и тип документа. Только для чтения       |

## <a name="relationships"></a>Отношения

| Свойство      | Тип          | Описание  |
| ------------- |---------------| -------------|
| resource      | Коллекция объектов | Используется для перехода к элементу, к которому предоставлен общий доступ. Для вложений в файл используется тип *fileAttachment*. Для связанных вложений используется тип *driveItem*. |

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
