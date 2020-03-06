---
title: Тип ресурса ресурсе resourcevisualization
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 876acf56d4f3445d55163a8c4cdb5bc1461c45de
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531294"
---
# <a name="resourcevisualization-resource-type"></a>Тип ресурса ресурсе resourcevisualization

Пространство имен: microsoft.graph

Сложный тип, содержащий свойства [оффицеграфинсигхтс](officegraphinsights.md).

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
| title                 | Строка        | Текст заголовка элемента.               |
| type              | String        | Тип мультимедиа элемента. Можно использовать для фильтрации определенного файла на основе определенного типа. Ниже приведены поддерживаемые типы. |
| mediaType             | Строка        | Тип мультимедиа элемента. Может использоваться для фильтрации файлов определенного типа на основе поддерживаемых типов MIME MIME для устройства IANA. Обратите внимание, что поддерживаются не все типы MIME мультимедиа. |
| превиевимажеурл       | Строка        | URL-адрес, ведущая к изображению для предварительного просмотра элемента. |
| previewText           | Строка        | Предварительный текст для элемента. |
| контаинервебурл       | Строка        | Путь, начинающийся с папки, в которой хранится элемент. |
| контаинердисплайнаме  | Строка        | Строка, описывающая место хранения элемента. Например, имя сайта SharePoint или имя пользователя, идентифицирующее владельца OneDrive, в котором хранится элемент.  |
| контаинертипе         | Строка | Можно использовать для фильтрации по типу контейнера, в котором хранится файл. Например, site или Онедривебусинесс.       |

## <a name="type-property-values"></a>Ввод значений свойств
-   PowerPoint
-   Word
-   Excel
-   ]
-   OneNote
-   оненотепаже
-   InfoPath
-   Visio
-   Publisher
-   Project
-   Доступ
-   Почта
-   Расширения
-   Архив
-   Компьютеров
-   "Audio" (Аудио);
-   "Video" (Видео);
-   Изображение
-   Web
-   Текст
-   Xml
-   Story
-   екстерналконтент
-   Folder
-   Другие

Пример запроса:`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

## <a name="containertype-property-values"></a>значения свойств Контаинертипе
Поддерживаемые типы могут различаться в зависимости от контейнеров, из которых [оффицеграфинсигхтс](officegraphinsights.md) возвращает файлы. Например, только представление [шарединсигхт](insights-shared.md) возвращает файлы из "Dropbox", "Box" и "гдриве".

-   онедривебусинесс
-   Сайт
-   Почта
-   Оставляют
-   Box
-   гдриве

Пример запроса:`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`
