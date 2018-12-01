---
title: Тип ресурса resourceVisualization
description: Сложный тип, содержащий свойства средствами.
ms.openlocfilehash: 3ed61a8547e072938fc073d90f2592baf4c08fba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079873"
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
-   "Web" (Интернет);
-   Текст
-   Xml
-   Story
-   ExternalContent
-   Folder
-   Other (другие)

Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

## <a name="containertype-property-values"></a>значения свойств containerType
Поддерживаемые типы может отличаться в зависимости от контейнеров, с которых [возможность получения](insights.md) возвращает файлы. Например только сведений об [общих](insights-shared.md) возвращает файлы из 'Общего банка данных», «Поле» и «GDrive».

-   OneDriveBusiness
-   Сайт
-   Почта
-   Общего банка данных
-   Box
-   GDrive

Пример запроса:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`