---
title: Тип ресурса OneNote
description: Точка входа для ресурсов OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 5ed063fb485acdbd029a977ffb6cd721bf7085c8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561665"
---
# <a name="onenote-resource-type"></a>Тип ресурса OneNote

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Точка входа для ресурсов OneNote.

Все вызовы службы OneNote через API Microsoft Graph используют следующий корневой URL-адрес службы:

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

Местоположение может представлять собой записные книжки для пользователей в Office 365 или OneDrive для пользователей, групповых записных книжек или размещенных на сайте SharePoint записных книжек группы в Office 365. 

**Записные книжКи пользователя** Чтобы получить доступ к личным записным книжкам в OneDrive для бизнеса или OneDrive для бизнеса, используйте один из следующих URL-адресов:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

**Записные книжки для групп** Чтобы получить доступ к записным книжкам, принадлежащим группе, используйте следующий корневой URL-адрес службы:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
**Записные книжки сайта SharePoint** Чтобы получить доступ к записным книжкам, принадлежащим сайту группы SharePoint, используйте следующий корневой URL-адрес службы:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a>Authorization

Для получения сведений о разрешениях, необходимых для работы с API [](/graph/permissions-reference#notes-permissions)OneNote, ознакомьтесь с разрешениями для заметок.

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|notebooks|[](notebook.md) Коллекция записных книжек|Коллекция записных книжек OneNote, принадлежащих пользователю или группе. Только для чтения. Допускается значение null.|
|operations|Коллекция [Operation](onenoteoperation.md) |Состояние операций OneNote. Получение коллекции Operations не поддерживается, но вы можете получить состояние длительно выполняемых операций, если `Operation-Location` заголовок возвращается в ответе. Только для чтения. Допускается значение null.|
|pages|Коллекция [страниц](page.md)|Страницы во всех записных книжках OneNote, принадлежащие пользователю или группе.  Только для чтения. Допускается значение null.|
|resources|Коллекция [ресурсов](resource.md) |Изображение и другие файловые ресурсы на страницах OneNote. Получение коллекции ресурсов не поддерживается, но вы можете [получить двоичное содержимое определенного ресурса](resource.md). Только для чтения. Допускается значение null.|
|sectionGroups|Коллекция [sectionGroup](sectiongroup.md)|Группы разделов во всех записных книжках OneNote, принадлежащие пользователю или группе.  Только для чтения. Допускается значение null.|
|sections|Коллекция [section](section.md)|Разделы во всех записных книжках OneNote, принадлежащие пользователю или группе.  Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание записной книжки](../api/onenote-post-notebooks.md) |[Notebook](notebook.md)| Создание записной книжки путем публикации в коллекции записных книжек.|
|[Список записных книжек](../api/onenote-list-notebooks.md) |[](notebook.md) Коллекция записных книжек| Получение коллекции записных книжек.|
|[Создание страницы](../api/onenote-post-pages.md) |[Page](page.md)| Создание страницы путем публикации в коллекции Pages.|
|[Перечисление страниц](../api/onenote-list-pages.md) |Коллекция [страниц](page.md)| Получение коллекции страниц.|
|[Список групп разделов](../api/onenote-list-sectiongroups.md) |Коллекция [sectionGroup](sectiongroup.md)| Получение коллекции групп разделов.|
|[Вывод списка разделов](../api/onenote-list-sections.md) |Коллекция [section](section.md)| Получение коллекции разделов.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenote.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
