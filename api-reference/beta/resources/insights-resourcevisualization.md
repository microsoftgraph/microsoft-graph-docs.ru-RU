---
title: Тип ресурса resourceVisualization
description: Сложный тип, содержащий свойства средствами.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 7600c843e36e3bce6c8a4182e0bfda14ad21d7b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844978"
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
| Тип носителя             | Строка        | Тип элемента мультимедиа. Можно использовать для фильтрации для определенного типа файлов, поддерживаемые типы Mime IANA мультимедиа на основании. Обратите внимание, что не все типы Mime мультимедиа поддерживаются. |
| previewImageUrl       | Строка        | URL-адрес, приводя к изображения предварительного просмотра для элемента. |
| previewText           | Строка        | Предварительная версия текст для элемента. |
| containerWebUrl       | Строка        | Путь, приводя к папке, в которой хранится элемент. |
| containerDisplayName  | Строка        | Строка, описывающая, где хранится элемент. Например имя сайт SharePoint или имя пользователя, определение владельца OneDrive, хранения элемента.  |
| containerType         | Строка | Можно использовать для фильтрации по типу контейнер, в котором хранится файл. Например, сайта или OneDriveBusiness.       |

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
-   Веб
-   Текст
-   Xml
-   Story
-   ExternalContent
-   Folder
-   Другое

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
