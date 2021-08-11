---
title: тип ресурса resourceVisualization
description: Сложный тип, содержащий свойства Аналитика.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a8f5d97a41e28e103d6cf756bb08790deef8c1ee0fa4a44b40a363bc759cf8ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126573"
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
| type              | String        | Тип мультимедиа элемента. Можно использовать для фильтрации для определенного файла на основе определенного типа. Ниже приведены поддерживаемые типы. |
| MediaType             | String        | Тип мультимедиа элемента. Может использоваться для фильтрации для определенного типа файла на основе поддерживаемых типов Mime IANA Media. Обратите внимание, что не все типы Mime мультимедиа поддерживаются. |
| previewImageUrl       | String        | URL-адрес, ведущий к изображению предварительного просмотра элемента. |
| previewText           | String        | Текст предварительного просмотра элемента. |
| containerWebUrl       | String        | Путь, ведущий к папке, в которой хранится элемент. |
| containerDisplayName  | String        | Строка, описываемая, где хранится элемент. Например, имя веб-SharePoint или имя пользователя, определяющие владельца OneDrive хранения элемента.  |
| containerType         | String | Можно использовать для фильтрации по типу контейнера, в котором хранится файл. Например, Site или OneDriveBusiness.       |

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
-   Access
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
-   Другие

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

