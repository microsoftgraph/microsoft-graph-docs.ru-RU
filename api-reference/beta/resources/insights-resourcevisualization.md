---
title: Тип ресурса ресурсе resourcevisualization
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 7eddc083bd38c0902f61d326926c86f48ca78714
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620912"
---
# <a name="resourcevisualization-resource-type"></a>Тип ресурса ресурсе resourcevisualization

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип, содержащий свойства [аналитики](officegraphinsights.md).

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
| type              | String        | Тип мультимедиа элемента. Можно использовать для фильтрации определенного файла на основе определенного типа. Ниже приведены поддерживаемые типы. |
| mediaType             | String        | Тип мультимедиа элемента. Может использоваться для фильтрации файлов определенного типа на основе поддерживаемых типов MIME MIME для устройства IANA. Обратите внимание, что поддерживаются не все типы MIME мультимедиа. |
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
-   Other

Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

## <a name="containertype-property-values"></a>значения свойств Контаинертипе
Поддерживаемые типы могут различаться в зависимости от контейнеров, из которых [оффицеграфинсигхтс](officegraphinsights.md) возвращает файлы. Например, только представление [шарединсигхт](insights-shared.md) возвращает файлы из "Dropbox", "Box" и "гдриве".

-   Онедривебусинесс
-   Site
-   Почта
-   Оставляют
-   Box
-   Гдриве

Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`
