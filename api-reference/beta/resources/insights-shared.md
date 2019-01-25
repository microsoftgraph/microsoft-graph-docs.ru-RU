---
title: Тип ресурса Shared
description: 'Возможность получения, представляющих файлы совместно с помощью или отдельного пользователя. Поддерживаются следующие общие файлы:'
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 11a6989e0130e7eedca7fff6f6cc9790d8109d84
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524690"
---
# <a name="shared-resource-type"></a>Тип ресурса Shared

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Возможность получения, представляющих файлы совместно с помощью или отдельного пользователя. Поддерживаются следующие общие файлы:

- Приглашение файлами, вложенными непосредственно в сообщение электронной почты или встрече.
- OneDrive для Bussiness и SharePoint современных вложения - файлов, хранящихся в OneDrive для бизнеса и SharePoint, которые пользователи совместно использовать как ссылки в сообщении электронной почты.

**Примечание**: Корпорация Майкрософт в настоящее время работает на заполнение результатов API совместно с данными. Возможно, некоторые данные, отсутствующие в первой недели после выпуска.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Список общих](../api/insights-list-shared.md) |[insights_shared](insights-shared.md) коллекции| Получите список общих файлов.|

## <a name="properties"></a>Свойства

| Свойство              | Тип                      | Описание  |
| -------------         |---------------            | -------------|
| id                    | String                    | Уникальный идентификатор связи. Только для чтения.        |
| lastShared            | [sharingDetail](insights-sharingdetail.md)                | Сведения об общих элементов. Только для чтения.        |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | Свойства, которые можно использовать для визуализации документа в работу. Только чтение      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Свойства ссылки общих документов, таких как URL-адрес и тип документа. Только чтение       |

## <a name="relationships"></a>Отношения

| Свойство      | Тип          | Описание  |
| ------------- |---------------| -------------|
| resource      | Entity        | Используется для перехода к элементу, предоставлен общий доступ. Для файлов вложений тип — *fileAttachment*. Для связанного вложения тип — *driveItem*. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
