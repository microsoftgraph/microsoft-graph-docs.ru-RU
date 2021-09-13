---
title: тип ресурса resourceVisualization
description: Сложный тип, содержащий свойства Аналитика.
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: e35848be021df48cb2ff10533bf597e91e58db24
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109159"
---
# <a name="resourcevisualization-resource-type"></a>тип ресурса resourceVisualization

Пространство имен: microsoft.graph

Сложный тип, содержащий свойства [officeGraphInsights.](officegraphinsights.md)

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],  
  "@odata.type": "microsoft.graph.resourceVisualization"
}-->
```json
{
  "title": "string",
  "type"  : "string",
  "mediaType": "string",
  "previewImageUrl": "string",
  "previewText": "string",
  "containerWebUrl": "string",
  "containerDisplayName": "string",
  "containerType": "string"
}
```

## <a name="properties"></a>Свойства

| Свойство              | Тип          | Описание  |
| -------------         |---------------| -------------|
| title                 | String        | Текст заголовка элемента.               |
| type              | Строка        | Тип мультимедиа элемента. Можно использовать для фильтрации для определенного файла на основе определенного типа. Ниже приведены поддерживаемые типы. |
| MediaType             | Строка        | Тип мультимедиа элемента. Может использоваться для фильтрации для определенного типа файла на основе поддерживаемых типов Mime IANA Media. Обратите внимание, что не все типы Mime мультимедиа поддерживаются. |
| previewImageUrl       | String        | URL-адрес, ведущий к изображению предварительного просмотра элемента. |
| previewText           | String        | Текст предварительного просмотра элемента. |
| containerWebUrl       | String        | Путь, ведущий к папке, в которой хранится элемент. |
| containerDisplayName  | Строка        | Строка, описываемая, где хранится элемент. Например, имя веб-SharePoint или имя пользователя, определяющие владельца OneDrive хранения элемента.  |
| containerType         | Строка | Можно использовать для фильтрации по типу контейнера, в котором хранится файл. Например, Site или OneDriveBusiness.       |

## <a name="type-property-values"></a>Тип значений свойств
-   PowerPoint
-   Word
-   Excel
-   Pdf
-   OneNote
-   OneNotePage
-   InfoPath
-   Visio
-   Publisher
-   Project
-   Доступ
-   Почта
-   Csv
-   Архив
-   Xps
-   "Audio" (Аудио);
-   "Video" (Видео);
-   Изображение
-   Web
-   Текст
-   Xml
-   Story
-   ExternalContent
-   Folder
- Spsite
-   Прочее

Пример запроса: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

Примечания: Для получения допустимых результатов может потребоваться сортировка `spsite` `lastUsed/lastAccessedDateTime` по desc

## <a name="containertype-property-values"></a>Значения свойств containerType
Поддерживаемые типы могут отличаться в зависимости от контейнеров, из которых [officeGraphInsights](officegraphinsights.md) возвращает файлы. Например, только понимание [sharedInsight](insights-shared.md) возвращает файлы из "DropBox", "Box" и "GDrive".

-   OneDriveBusiness
-   Site
-   Почта
-   DropBox
-   Box
-   GDrive

Пример запроса: `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

