---
title: Работа с сайтами SharePoint в Microsoft Graph
description: 'API SharePoint в Microsoft Graph поддерживает следующие основные сценарии:'
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 9edab0f8e4207dac2a88943a0a2cd1cbe58b97e3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945736"
---
# <a name="working-with-sharepoint-sites-in-microsoft-graph"></a><span data-ttu-id="a4a11-103">Работа с сайтами SharePoint в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a4a11-103">Working with SharePoint sites in Microsoft Graph</span></span>

<span data-ttu-id="a4a11-104">API SharePoint в Microsoft Graph поддерживает следующие основные сценарии:</span><span class="sxs-lookup"><span data-stu-id="a4a11-104">The SharePoint API in Microsoft Graph supports the following core scenarios:</span></span>

* <span data-ttu-id="a4a11-105">доступ к ресурсам **site**, **list** и **drive** (библиотекам документов) в SharePoint;</span><span class="sxs-lookup"><span data-stu-id="a4a11-105">Access to SharePoint **sites**, **lists**, and **drives** (document libraries)</span></span>
* <span data-ttu-id="a4a11-106">доступ к ресурсам **site** только для чтения (без возможности создавать сайты);</span><span class="sxs-lookup"><span data-stu-id="a4a11-106">Read-only support for **site** resources (no ability to create new sites)</span></span>
* <span data-ttu-id="a4a11-107">доступ на чтение и запись к ресурсам **list**, **listItem** и **driveItem**;</span><span class="sxs-lookup"><span data-stu-id="a4a11-107">Read-write support for **lists**, **listItems**, and **driveItems**</span></span>
* <span data-ttu-id="a4a11-108">обращение к ресурсам по идентификатору SharePoint, URL-адресу или относительному пути.</span><span class="sxs-lookup"><span data-stu-id="a4a11-108">Address resources by SharePoint ID, URL, or relative path</span></span>

<span data-ttu-id="a4a11-109">API SharePoint предоставляет три основных типа ресурсов:</span><span class="sxs-lookup"><span data-stu-id="a4a11-109">The SharePoint API exposes three major resource types:</span></span>

* <span data-ttu-id="a4a11-110">[Site](site.md) _(объект верхнего уровня)_</span><span class="sxs-lookup"><span data-stu-id="a4a11-110">[Site](site.md) _(top-level object)_</span></span>
* <span data-ttu-id="a4a11-111">[List](list.md);</span><span class="sxs-lookup"><span data-stu-id="a4a11-111">[List](list.md)</span></span>
* <span data-ttu-id="a4a11-112">[ListItem](listitem.md).</span><span class="sxs-lookup"><span data-stu-id="a4a11-112">[ListItem](listitem.md)</span></span>

<span data-ttu-id="a4a11-113">Ниже показан пример ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="a4a11-113">The following is an example of a listItem resource.</span></span>

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

<span data-ttu-id="a4a11-114">Ресурсы предоставляют данные тремя разными способами:</span><span class="sxs-lookup"><span data-stu-id="a4a11-114">Resources expose data in three different ways:</span></span>

* <span data-ttu-id="a4a11-115">_Свойства_ (например, **id** и **name**) предоставляют простые значения.</span><span class="sxs-lookup"><span data-stu-id="a4a11-115">_Properties_ (like **id** and **name**) expose simple values.</span></span>
* <span data-ttu-id="a4a11-116">_Аспекты_ (например, **fields** и **createdBy**) предоставляют сложные значения.</span><span class="sxs-lookup"><span data-stu-id="a4a11-116">_Facets_ (like **fields** and **createdBy**) expose complex values.</span></span>
* <span data-ttu-id="a4a11-117">_Ссылки_ (например, **items**) указывают на коллекции других ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a4a11-117">_References_ (like **items**) point to collections of other resources.</span></span>

<span data-ttu-id="a4a11-118">Вы можете расширить ссылки в URL-адресе с помощью параметра запроса _expand_, например `?expand=fields`.</span><span class="sxs-lookup"><span data-stu-id="a4a11-118">You can expand references in your URL with the _expand_ query parameter; for example, `?expand=fields`.</span></span>
<span data-ttu-id="a4a11-119">Вы можете запросить определенные свойства и аспекты с помощью параметра запроса _select_, например `?select=id,name`.</span><span class="sxs-lookup"><span data-stu-id="a4a11-119">You can request specific properties and facets with the _select_ query parameter; for example, `?select=id,name`.</span></span>
<span data-ttu-id="a4a11-120">По умолчанию возвращается большая часть свойств и аспектов, при этом все ссылки скрыты.</span><span class="sxs-lookup"><span data-stu-id="a4a11-120">By default, most properties and facets are returned while all references are hidden.</span></span>
<span data-ttu-id="a4a11-121">Для повышения эффективности мы рекомендуем указывать операторы _select_ и _expand_, чтобы возвращать только важные для вас данные.</span><span class="sxs-lookup"><span data-stu-id="a4a11-121">For efficiency, we recommend that you specify _select_ and _expand_ to only return the data you care about.</span></span>

## <a name="sharepoint-api-root-resources"></a><span data-ttu-id="a4a11-122">Корневые ресурсы API SharePoint</span><span class="sxs-lookup"><span data-stu-id="a4a11-122">SharePoint API root resources</span></span>

<span data-ttu-id="a4a11-123">Приведенные ниже примеры относятся к `https://graph.microsoft.com/beta`.</span><span class="sxs-lookup"><span data-stu-id="a4a11-123">The following examples are relative to `https://graph.microsoft.com/beta`.</span></span>

| <span data-ttu-id="a4a11-124">Путь</span><span class="sxs-lookup"><span data-stu-id="a4a11-124">Path</span></span>                                   | <span data-ttu-id="a4a11-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a4a11-125">Description</span></span>
|:---------------------------------------|:------------------------------------
| <span data-ttu-id="a4a11-126">/sites/root</span><span class="sxs-lookup"><span data-stu-id="a4a11-126">/sites/root</span></span>                            | <span data-ttu-id="a4a11-127">Ресурс [site][] по умолчанию для организации.</span><span class="sxs-lookup"><span data-stu-id="a4a11-127">Organization's default [site][].</span></span>
| <span data-ttu-id="a4a11-128">/sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="a4a11-128">/sites/{site-id}</span></span>                       | <span data-ttu-id="a4a11-129">Доступ к определенному ресурсу [site][] с использованием его идентификатора.</span><span class="sxs-lookup"><span data-stu-id="a4a11-129">Access a specific [site][] by its ID.</span></span>
| <span data-ttu-id="a4a11-130">/sites/{site-id}/drive</span><span class="sxs-lookup"><span data-stu-id="a4a11-130">/sites/{site-id}/drive</span></span>                 | <span data-ttu-id="a4a11-131">Доступ к ресурсу [drive](drive.md) (библиотеке документов) для указанного ресурса [site][], заданному по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a4a11-131">Access the default [drive](drive.md) (document library) for the given [site][].</span></span>
| <span data-ttu-id="a4a11-132">/sites/{site-id}/drives</span><span class="sxs-lookup"><span data-stu-id="a4a11-132">/sites/{site-id}/drives</span></span>                | <span data-ttu-id="a4a11-133">Перечисление ресурсов [drive](drive.md) (библиотек документов) для [site][].</span><span class="sxs-lookup"><span data-stu-id="a4a11-133">Enumerate the [drives](drive.md) (document libraries) under the [site][].</span></span>
| <span data-ttu-id="a4a11-134">/sites/{site-id}/sites</span><span class="sxs-lookup"><span data-stu-id="a4a11-134">/sites/{site-id}/sites</span></span>                 | <span data-ttu-id="a4a11-135">Перечисление дочерних сайтов для ресурса [site][].</span><span class="sxs-lookup"><span data-stu-id="a4a11-135">Enumerate the sub-sites under the [site][].</span></span>
| <span data-ttu-id="a4a11-136">/sites/{site-id}/lists</span><span class="sxs-lookup"><span data-stu-id="a4a11-136">/sites/{site-id}/lists</span></span>                 | <span data-ttu-id="a4a11-137">Перечисление ресурсов [lists](list.md) для ресурса [site](site.md).</span><span class="sxs-lookup"><span data-stu-id="a4a11-137">Enumerate the [lists](list.md) under the [site](site.md).</span></span>
| <span data-ttu-id="a4a11-138">/sites/{site-id}/lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="a4a11-138">/sites/{site-id}/lists/{list-id}/items</span></span> | <span data-ttu-id="a4a11-139">Перечисление ресурсов [listItem](listitem.md) для ресурса [list](list.md).</span><span class="sxs-lookup"><span data-stu-id="a4a11-139">Enumerate the [listItems](listitem.md) under the [list](list.md).</span></span>
| <span data-ttu-id="a4a11-140">/groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="a4a11-140">/groups/{group-id}/sites/root</span></span>          | <span data-ttu-id="a4a11-141">Доступ к [сайту][] группы для группы.</span><span class="sxs-lookup"><span data-stu-id="a4a11-141">Access a group's team [site][].</span></span>

<span data-ttu-id="a4a11-p102">К сайту также можно обратиться с помощью соответствующего пути. Для этого укажите имя узла SharePoint, за ним — двоеточие и относительный путь к сайту. При необходимости вы можете менять способ адресации (возвращаться к ресурсной модели), добавляя в конец двоеточие.</span><span class="sxs-lookup"><span data-stu-id="a4a11-p102">Sites can also be addressed by path by using the SharePoint hostname, followed by a colon and the relative path to the site. You can optionally transition back to addressing the resource model by putting another colon at the end.</span></span>

| <span data-ttu-id="a4a11-144">Путь</span><span class="sxs-lookup"><span data-stu-id="a4a11-144">Path</span></span>                                           | <span data-ttu-id="a4a11-145">Описание</span><span class="sxs-lookup"><span data-stu-id="a4a11-145">Description</span></span>
|:-----------------------------------------------|:-----------------------------------
| <span data-ttu-id="a4a11-146">/sites/contoso.sharepoint.com:/teams/hr</span><span class="sxs-lookup"><span data-stu-id="a4a11-146">/sites/contoso.sharepoint.com:/teams/hr</span></span>        | <span data-ttu-id="a4a11-147">Сайт, связанный сhttps://contoso.sharepoint.com/teams/hr</span><span class="sxs-lookup"><span data-stu-id="a4a11-147">The site associated with https://contoso.sharepoint.com/teams/hr</span></span>
| <span data-ttu-id="a4a11-148">/sites/contoso.sharepoint.com:/teams/hr:/drive</span><span class="sxs-lookup"><span data-stu-id="a4a11-148">/sites/contoso.sharepoint.com:/teams/hr:/drive</span></span> | <span data-ttu-id="a4a11-149">Доступ к ресурсу [drive](drive.md), заданному по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a4a11-149">Access the default [drive](drive.md) for this site.</span></span>

## <a name="note-for-existing-sharepoint-developers"></a><span data-ttu-id="a4a11-150">Примечание, касающееся разработки решений для SharePoint</span><span class="sxs-lookup"><span data-stu-id="a4a11-150">Note for existing SharePoint developers</span></span>

<span data-ttu-id="a4a11-p103">API SharePoint в Microsoft Graph имеет ряд ключевых отличий от API CSOM. Ресурс [site][] сопоставляется с `SPWeb`. Корневой ресурс [site][] (`SPWeb`) в семействе веб-сайтов имеет аспект [siteCollection](sitecollection.md), содержащий сведения о `SPSite`. Идентификатор сайта уникален только в пределах одного семейства веб-сайтов. Чтобы обратиться к сайту с использованием ИД, нужно предоставить два идентификатора — для семейства и для самого сайта.</span><span class="sxs-lookup"><span data-stu-id="a4a11-p103">The Microsoft Graph SharePoint API has a few key differences with the CSOM APIs. The [site][] resource maps to `SPWeb`. The root [site][] (`SPWeb`) in a site collection has a [siteCollection](sitecollection.md) facet, which contains information about the `SPSite`. Because IDs for sites are only unique within their site collection, addressing a site by ID requires providing both the site collection identifier and the site identifier.</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{hostname},{spsite-id},{spweb-id}/
```
<span data-ttu-id="a4a11-155">URL-адрес, содержащий только имя узла, будет указывать на корневой сайт (`SPWeb`) в семействе веб-сайтов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a4a11-155">A URL constructed with only the hostname will point to the root site (`SPWeb`) in the default site collection.</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{hostname}
```

<span data-ttu-id="a4a11-156">URL-адрес, содержащий только имя узла и идентификатор siteCollection (`SPSite`), будет указывать на корневой сайт (`SPWeb`) в указанном семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="a4a11-156">A URL constructed with only the hostname and siteCollection (`SPSite`) ID will point to the root site (`SPWeb`) in the given site collection.</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{hostname},{spsite-id}
```

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
