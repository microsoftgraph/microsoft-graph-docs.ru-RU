---
title: Тип ресурса resourceVisualization
description: Сложный тип, содержащий свойства средствами.
author: simonhult
ms.openlocfilehash: d0c54895468fc9a01017e448df57c09c654616e9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333539"
---
# <a name="resourcevisualization-resource-type"></a>Тип ресурса resourceVisualization

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
| title                 | Строка        | Текст заголовка элемента.               |
| type              | Строка        | Тип элемента мультимедиа. Можно использовать для фильтрации для конкретного файла на основе определенного типа. Ниже приведены поддерживаемые типы. |
| Тип носителя             | String.        | Тип элемента мультимедиа. Можно использовать для фильтрации для определенного типа файлов, поддерживаемые типы Mime IANA мультимедиа на основании. Обратите внимание, что не все типы Mime мультимедиа поддерживаются. |
| previewImageUrl       | String.        | URL-адрес, приводя к изображения предварительного просмотра для элемента. |
| previewText           | String.        | Предварительная версия текст для элемента. |
| containerWebUrl       | String.        | Путь, приводя к папке, в которой хранится элемент. |
| containerDisplayName  | String.        | Строка, описывающая, где хранится элемент. Например имя сайт SharePoint или имя пользователя, определение владельца OneDrive, хранения элемента.  |
| containerType         | String. | Можно использовать для фильтрации по типу контейнер, в котором хранится файл. Например, сайта или OneDriveBusiness.       |

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