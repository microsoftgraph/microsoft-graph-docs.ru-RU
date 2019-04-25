---
title: Тип ресурса ресурсе resourcevisualization
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ec1619d07d0f31bf8325c25b161084f505b3ee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550740"
---
# <a name="resourcevisualization-resource-type"></a>Тип ресурса ресурсе resourcevisualization

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип, содержащий свойства [аналитики](insights.md).

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
| type              | String        | Тип мультимедиа элемента. Можно использовать для фильтрации определенного файла на основе определенного типа. Ниже приведены поддерживаемые типы. |
| mediaType             | String        | Тип мультимедиа элемента. Может использоваться для фильтрации для определенного типа файлов на основе поддерживаемых типов MIME для мультимедиа IANA. Обратите внимание, что поддерживаются не все типы MIME мультимедиа. |
| Превиевимажеурл       | String        | URL-адрес, ведущая к изображению для предварительного просмотра элемента. |
| previewText           | String        | Предварительный текст для элемента. |
| Контаинервебурл       | String        | Путь, начинающийся с папки, в которой хранится элемент. |
| Контаинердисплайнаме  | String        | Строка, описывающая место хранения элемента. Например, имя сайта SharePoint или имя пользователя, идентифицирующее владельца OneDrive, в котором хранится элемент.  |
| Контаинертипе         | String | Можно использовать для фильтрации по типу контейнера, в котором хранится файл. Например, site или Онедривебусинесс.       |

## <a name="type-property-values"></a>Ввод значений свойств
-   PowerPoint
-   Word
-   Excel
-   ]
-   OneNote
-   Оненотепаже
-   InfoPath
-   Visio
-   Publisher
-   Project
-   Access
-   Почта
-   Расширения
-   Архив
-   Компьютеров
-   "Audio" (Аудио);
-   "Video" (Видео);
-   Изображение
-   Веб
-   Текст
-   Xml
-   Story
-   Екстерналконтент
-   Folder
-   Другие

Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

## <a name="containertype-property-values"></a>значения свойств Контаинертипе
Поддерживаемые типы могут различаться в зависимости от контейнера, из [](insights.md) которого возвращаются файлы. Например, только [Общие](insights-shared.md) сведения о файлах "Dropbox", "Box" и "гдриве".

-   Онедривебусинесс
-   Сайт
-   Почта
-   Оставляют
-   Box
-   Гдриве

Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
