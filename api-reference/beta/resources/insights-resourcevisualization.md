---
title: Тип ресурса ресурсе resourcevisualization
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: cb782ff0090c5e89e4a87f86af75f3fb51bb8251
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495657"
---
# <a name="resourcevisualization-resource-type"></a>Тип ресурса ресурсе resourcevisualization

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| title                 | String        | Текст заголовка элемента.               |
| type              | String        | Тип мультимедиа элемента. Можно использовать для фильтрации определенного файла на основе определенного типа. Ниже приведены поддерживаемые типы. |
| mediaType             | String        | Тип мультимедиа элемента. Может использоваться для фильтрации файлов определенного типа на основе поддерживаемых типов MIME MIME для устройства IANA. Обратите внимание, что поддерживаются не все типы MIME мультимедиа. |
| превиевимажеурл       | String        | URL-адрес, ведущая к изображению для предварительного просмотра элемента. |
| previewText           | String        | Предварительный текст для элемента. |
| контаинервебурл       | String        | Путь, начинающийся с папки, в которой хранится элемент. |
| контаинердисплайнаме  | String        | Строка, описывающая место хранения элемента. Например, имя сайта SharePoint или имя пользователя, идентифицирующее владельца OneDrive, в котором хранится элемент.  |
| контаинертипе         | String | Можно использовать для фильтрации по типу контейнера, в котором хранится файл. Например, site или Онедривебусинесс.       |

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

Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

## <a name="containertype-property-values"></a>значения свойств Контаинертипе
Поддерживаемые типы могут различаться в зависимости от контейнеров, из которых [оффицеграфинсигхтс](officegraphinsights.md) возвращает файлы. Например, только представление [шарединсигхт](insights-shared.md) возвращает файлы из "Dropbox", "Box" и "гдриве".

-   онедривебусинесс
-   Сайт
-   Почта
-   Оставляют
-   Box
-   гдриве

Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`
