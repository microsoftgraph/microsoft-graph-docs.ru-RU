---
title: Тип ресурса onenote
description: Точка входа для ресурсов OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: e213f12110399b90513d33af4d1745be3cdf3eae
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898067"
---
# <a name="onenote-resource-type"></a>Тип ресурса onenote

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Точка входа для ресурсов OneNote.

Все вызовы службы OneNote через API Microsoft Graph выполняются с помощью следующего корневого URL-адреса службы:

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

Местоположение может представлять собой записные книжки для пользователей в Microsoft 365 или OneDrive для пользователей, групповые записные книжки или записные книжки группы SharePoint, размещенные на сайте Microsoft 365. 

**Записные книжки пользователей.** Чтобы получить доступ к персональным записным книжкам в OneDrive для бизнеса или личном хранилище OneDrive, воспользуйтесь одним из следующих URL-адресов:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

**Записные книжки группы.** Чтобы получить доступ к записным книжкам группы, воспользуйтесь следующим корневым URL-адресом службы:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
**Записные книжки на сайте SharePoint.** Чтобы получить доступ к записным книжкам на сайте группы SharePoint, воспользуйтесь следующим корневым URL-адресом службы:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a>Авторизация

Сведения о разрешениях, необходимых для работы с API OneNote, см. в разделе [Разрешения для заметок](/graph/permissions-reference#notes-permissions).

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|notebooks|Коллекция объектов [notebook](notebook.md)|Коллекция записных книжек OneNote, принадлежащих пользователю или группе. Только для чтения. Допускается значение null.|
|operations|Коллекция [onenoteOperation](onenoteoperation.md) |Состояние операций OneNote. Получение коллекции операций не поддерживается, но можно получить состояние длительных операций, если в отклике возвращается заголовок `Operation-Location`. Только для чтения. Допускается значение null.|
|pages|Коллекция [оненотепаже](onenotepage.md)|Страницы всех записных книжек OneNote, принадлежащих пользователю или группе.  Только для чтения. Допускается значение null.|
|resources|Коллекция [оненотересаурце](onenoteresource.md) |Изображения и другие файловые ресурсы на страницах OneNote. Получение коллекции ресурсов не поддерживается, но можно [получить двоичное содержимое определенного ресурса](onenoteresource.md). Только для чтения. Допускается значение null.|
|sectionGroups|Коллекция [sectionGroup](sectiongroup.md)|Группы разделов во всех записных книжках OneNote, принадлежащих пользователю или группе.  Только для чтения. Допускает значение null.|
|sections|Коллекция [оненотесектион](onenotesection.md)|Разделы во всех записных книжках OneNote, принадлежащих пользователю или группе.  Только для чтения. Допускается значение null.|

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание записной книжки](../api/onenote-post-notebooks.md) |[notebook](notebook.md)| Создание записной книжки путем публикации в коллекции записных книжек.|
|[Перечисление записных книжек](../api/onenote-list-notebooks.md) |Коллекция объектов [notebook](notebook.md)| Получение коллекции записных книжек.|
|[Создание страницы](../api/onenote-post-pages.md) |[оненотепаже](onenotepage.md) | Создание страницы путем публикации в коллекции страниц.|
|[Перечисление страниц](../api/onenote-list-pages.md) |Коллекция [оненотепаже](onenotepage.md)| Получение коллекции страниц.|
|[Перечисление групп разделов](../api/onenote-list-sectiongroups.md) |Коллекция [sectionGroup](sectiongroup.md)| Получение коллекции групп разделов.|
|[Перечисление разделов](../api/onenote-list-sections.md) |Коллекция [оненотесектион](onenotesection.md)| Получение коллекции разделов.|
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenote"
}-->
``` json
{
  "notebooks": [{ "@odata.type": "microsoft.graph.notebook" }],
  "operations": [{ "@odata.type": "microsoft.graph.onenoteOperation" }],
  "pages": [{ "@odata.type": "microsoft.graph.onenotePage" }],
  "resources": [ { "@odata.type": "microsoft.graph.onenoteResource" } ],
  "sectionGroups": [ { "@odata.type": "microsoft.graph.sectionGroup" } ],
  "sections": [ { "@odata.type": "microsoft.graph.onenoteSection" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
