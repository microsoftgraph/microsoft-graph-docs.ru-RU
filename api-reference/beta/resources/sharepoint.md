---
title: Работа с сайтами SharePoint в Microsoft Graph
description: 'API SharePoint в Microsoft Graph поддерживает следующие основные сценарии:'
ms.localizationpriority: high
ms.prod: sharepoint
doc_type: conceptualPageType
author: JeremyKelley
ms.openlocfilehash: efa5ff08f54a7bca493f14a37f6a665b9bd0492c
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/30/2021
ms.locfileid: "58694614"
---
# <a name="working-with-sharepoint-sites-in-microsoft-graph"></a>Работа с сайтами SharePoint в Microsoft Graph

API SharePoint в Microsoft Graph поддерживает следующие основные сценарии:

* доступ к ресурсам **site**, **list** и **drive** (библиотекам документов) в SharePoint;
* доступ к ресурсам **site** только для чтения (без возможности создавать сайты);
* доступ на чтение и запись к ресурсам **list**, **listItem** и **driveItem**;
* обращение к ресурсам по идентификатору SharePoint, URL-адресу или относительному пути.

API SharePoint предоставляет три основных типа ресурсов:

* [Site](site.md) _(объект верхнего уровня)_
* [List](list.md)
* [ListItem](listitem.md)

Ниже показан пример ресурса listItem.

```json
{
  "fields": {
    "Title": "Access card",
    "Employee": "Ryan Gregg",
    "EmployeeId": "10",
    "CardSerial": "01235492",
    "Alias": "RGregg",
    "ID": 1,
    "ContentType": "Item",
    "Modified": "2016-09-19T23:15:25-07:00",
    "Created": "2016-09-19T23:15:25-07:00"
  },
  "createdBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "createdDateTime": "2016-09-20T06:15:25Z",
  "eTag": "48e941c3-9515-4c48-9760-c07c90c79d48,1",
  "id": "4",
  "lastModifiedBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "lastModifiedDateTime": "2016-09-20T06:15:25Z",
}
```

Ресурсы предоставляют данные тремя разными способами:

* _Свойства_ (например, **id** и **name**) предоставляют простые значения.
* _Аспекты_ (например, **fields** и **createdBy**) предоставляют сложные значения.
* _Ссылки_ (например, **items**) указывают на коллекции других ресурсов.

Вы можете расширить ссылки в URL-адресе с помощью параметра запроса _expand_, например `?expand=fields`.
Вы можете запросить определенные свойства и аспекты с помощью параметра запроса _select_, например `?select=id,name`.
По умолчанию возвращается большая часть свойств и аспектов, при этом все ссылки скрыты.
Для повышения эффективности мы рекомендуем указывать операторы _select_ и _expand_, чтобы возвращать только важные для вас данные.

## <a name="sharepoint-api-root-resources"></a>Корневые ресурсы API SharePoint

Приведенные ниже примеры относятся к `https://graph.microsoft.com/beta`.

| Путь                                   | Описание
|:---------------------------------------|:------------------------------------
| /sites/root                            | Ресурс [site][] по умолчанию для организации.
| /sites/{site-id}                       | Доступ к определенному ресурсу [site][] с использованием его идентификатора.
| /sites/{site-id}/drive                 | Доступ к ресурсу [drive](drive.md) (библиотеке документов) для указанного ресурса [site][], заданному по умолчанию.
| /sites/{site-id}/drives                | Перечисление ресурсов [drive](drive.md) (библиотек документов) для [site][].
| /sites/{site-id}/sites                 | Перечисление дочерних сайтов для ресурса [site][].
| /sites/{site-id}/lists                 | Перечисление ресурсов [lists](list.md) для ресурса [site](site.md).
| /sites/{site-id}/lists/{list-id}/items | Перечисление ресурсов [listItem](listitem.md) для ресурса [list](list.md).
| /groups/{group-id}/sites/root          | Доступ к [сайту][] группы для группы.

К сайту также можно обратиться с помощью соответствующего пути. Для этого укажите имя узла SharePoint, за ним — двоеточие и относительный путь к сайту. При необходимости вы можете менять способ адресации (возвращаться к ресурсной модели), добавляя в конец двоеточие.

| Путь                                           | Описание
|:-----------------------------------------------|:-----------------------------------
| /sites/contoso.sharepoint.com:/teams/hr        | Сайт, связанный с https://contoso.sharepoint.com/teams/hr
| /sites/contoso.sharepoint.com:/teams/hr:/drive | Доступ к ресурсу [drive](drive.md), заданному по умолчанию.

## <a name="note-for-existing-sharepoint-developers"></a>Примечание, касающееся разработки решений для SharePoint

API SharePoint в Microsoft Graph имеет ряд ключевых отличий от API CSOM.
Ресурс [site][] сопоставляется с `SPWeb`.
Корневой ресурс [site][] (`SPWeb`) в семействе веб-сайтов имеет аспект [siteCollection](sitecollection.md), содержащий сведения о `SPSite`.
Идентификаторы сайтов уникальны только в пределах одного семейства веб-сайтов. Поэтому чтобы обратиться к сайту по его идентификатору, необходимо указать два идентификатора — для семейства веб-сайтов и для самого сайта.

```http
GET https://graph.microsoft.com/beta/sites/{hostname},{spsite-id},{spweb-id}/
```
URL-адрес, содержащий только имя узла, будет указывать на корневой сайт (`SPWeb`) в семействе веб-сайтов по умолчанию.

```http
GET https://graph.microsoft.com/beta/sites/{hostname}
```

URL-адрес, содержащий только имя узла и идентификатор siteCollection (`SPSite`), будет указывать на корневой сайт (`SPWeb`) в указанном семействе веб-сайтов.

```http
GET https://graph.microsoft.com/beta/sites/{hostname},{spsite-id}
```

## <a name="whats-new"></a>Что нового
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

[site]: site.md
[list]: list.md
[drive]: drive.md
[siteCollection]: sitecollection.md

<!-- {
  "type": "#page.annotation",
  "description": "Getting started programming with the SharePoint API",
  "keywords": "getting started sharepoint rest api programming C# ios android rest http",
  "section": "documentation",
  "tocPath": "Getting Started",
  "tocIndex": -100
} -->


