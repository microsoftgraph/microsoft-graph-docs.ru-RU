---
title: Тип ресурса resourceVisualization
description: Сложный тип, содержащий свойства средствами.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ec1619d07d0f31bf8325c25b161084f505b3ee
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641297"
---
# <a name="resourcevisualization-resource-type"></a>Тип ресурса resourceVisualization

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип, содержащий свойства [средствами](insights.md).

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

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
| type              | String        | Тип элемента мультимедиа. Можно использовать для фильтрации для конкретного файла на основе определенного типа. Ниже приведены поддерживаемые типы. |
| Тип носителя             | String        | Тип элемента мультимедиа. Можно использовать для фильтрации для определенного типа файлов, поддерживаемые типы Mime IANA мультимедиа на основании. Обратите внимание, что не все типы Mime мультимедиа поддерживаются. |
| previewImageUrl       | String        | URL-адрес, приводя к изображения предварительного просмотра для элемента. |
| previewText           | String        | Предварительная версия текст для элемента. |
| containerWebUrl       | String        | Путь, приводя к папке, в которой хранится элемент. |
| containerDisplayName  | String        | Строка, описывающая, где хранится элемент. Например имя сайт SharePoint или имя пользователя, определение владельца OneDrive, хранения элемента.  |
| containerType         | String | Можно использовать для фильтрации по типу контейнер, в котором хранится файл. Например, сайта или OneDriveBusiness.       |

## <a name="type-property-values"></a>Тип значения свойств
-   PowerPoint
-   Word
-   Excel
-   PDF
-   OneNote
-   OneNotePage
-   InfoPath
-   Visio
-   Publisher
-   Project
-   Access
-   Почта
-   CSV
-   Archive
-   XPS
-   Audio (аудио)
-   Video (видео)
-   Изображение
-   Web
-   Текст
-   Xml
-   Story
-   ExternalContent
-   Folder
-   Other

Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

## <a name="containertype-property-values"></a>значения свойств containerType
Поддерживаемые типы может отличаться в зависимости от контейнеров, с которых [возможность получения](insights.md) возвращает файлы. Например только сведений об [общих](insights-shared.md) возвращает файлы из 'Общего банка данных», «Поле» и «GDrive».

-   OneDriveBusiness
-   Site
-   Почта
-   Общего банка данных
-   Box
-   GDrive

Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
