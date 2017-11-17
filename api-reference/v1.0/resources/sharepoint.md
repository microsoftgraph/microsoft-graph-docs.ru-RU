# <a name="working-with-sharepoint-sites-in-microsoft-graph"></a><span data-ttu-id="c04e3-101">Работа с сайтами SharePoint в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="c04e3-101">Working with SharePoint sites in Microsoft Graph</span></span>

<span data-ttu-id="c04e3-102">API SharePoint в Microsoft Graph поддерживает следующие основные сценарии:</span><span class="sxs-lookup"><span data-stu-id="c04e3-102">The SharePoint API in Microsoft Graph supports the following core scenarios:</span></span>

* <span data-ttu-id="c04e3-103">доступ к ресурсам **site**, **list** и **drive** (библиотекам документов) в SharePoint;</span><span class="sxs-lookup"><span data-stu-id="c04e3-103">Access to SharePoint **sites**, **lists**, and **drives** (document libraries)</span></span>
* <span data-ttu-id="c04e3-104">доступ к ресурсам **site** только для чтения (без возможности создавать сайты);</span><span class="sxs-lookup"><span data-stu-id="c04e3-104">Read-only support for **site** resources (no ability to create new sites)</span></span>
* <span data-ttu-id="c04e3-105">доступ на чтение и запись к ресурсам **list**, **listItem** и **driveItem**;</span><span class="sxs-lookup"><span data-stu-id="c04e3-105">Read-write support for **lists**, **listItems**, and **driveItems**</span></span>
* <span data-ttu-id="c04e3-106">обращение к ресурсам по идентификатору SharePoint, URL-адресу или относительному пути.</span><span class="sxs-lookup"><span data-stu-id="c04e3-106">Address resources by SharePoint ID, URL, or relative path</span></span>

<span data-ttu-id="c04e3-107">API SharePoint предоставляет три основных типа ресурсов:</span><span class="sxs-lookup"><span data-stu-id="c04e3-107">The SharePoint API exposes three major resource types:</span></span>

* <span data-ttu-id="c04e3-108">[Site](site.md) _(объект верхнего уровня)_</span><span class="sxs-lookup"><span data-stu-id="c04e3-108">[Site](site.md) _(top-level object)_</span></span>
* [<span data-ttu-id="c04e3-109">List</span><span class="sxs-lookup"><span data-stu-id="c04e3-109">List</span></span>](list.md)
* [<span data-ttu-id="c04e3-110">ListItem</span><span class="sxs-lookup"><span data-stu-id="c04e3-110">ListItem</span></span>](listitem.md)

<span data-ttu-id="c04e3-111">Ниже показан пример ресурса listItem.</span><span class="sxs-lookup"><span data-stu-id="c04e3-111">The following is an example of a driveItem resource.</span></span>

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

<span data-ttu-id="c04e3-112">Ресурсы предоставляют данные тремя разными способами:</span><span class="sxs-lookup"><span data-stu-id="c04e3-112">Drive and DriveItem resources expose data in three different ways:</span></span>

* <span data-ttu-id="c04e3-113">_Свойства_ (например, **id** и **name**) предоставляют простые значения.</span><span class="sxs-lookup"><span data-stu-id="c04e3-113">_Properties_ (like **id** and **name**) expose simple values.</span></span>
* <span data-ttu-id="c04e3-114">_Аспекты_ (например, **fields** и **createdBy**) предоставляют сложные значения.</span><span class="sxs-lookup"><span data-stu-id="c04e3-114">_Facets_ (like **file** and **photo**) expose complex values.</span></span>
* <span data-ttu-id="c04e3-115">_Ссылки_ (например, **items**) указывают на коллекции других ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c04e3-115">_References_ (like **children**) point to collections of other resources.</span></span>

<span data-ttu-id="c04e3-116">Вы можете расширить ссылки в URL-адресе с помощью параметра запроса _expand_, например `?expand=fields`.</span><span class="sxs-lookup"><span data-stu-id="c04e3-116">You can expand references in your URL with the _expand_ query parameter; for example, `?expand=fields`.</span></span>
<span data-ttu-id="c04e3-117">Вы можете запросить определенные свойства и аспекты с помощью параметра запроса _select_, например `?select=id,name`.</span><span class="sxs-lookup"><span data-stu-id="c04e3-117">You can request specific properties and facets with the _select_ query parameter; for example, `?select=id,name`.</span></span>
<span data-ttu-id="c04e3-118">По умолчанию возвращается большая часть свойств и аспектов, при этом все ссылки скрыты.</span><span class="sxs-lookup"><span data-stu-id="c04e3-118">By default, most properties and facets are returned while all references are hidden.</span></span>
<span data-ttu-id="c04e3-119">Для повышения эффективности мы рекомендуем указывать операторы _select_ и _expand_, чтобы возвращать только важные для вас данные.</span><span class="sxs-lookup"><span data-stu-id="c04e3-119">For efficiency, we recommend that you specify _select_ and _expand_ for the data you care about.</span></span>

## <a name="sharepoint-api-root-resources"></a><span data-ttu-id="c04e3-120">Корневые ресурсы API SharePoint</span><span class="sxs-lookup"><span data-stu-id="c04e3-120">SharePoint API root resources</span></span>

<span data-ttu-id="c04e3-121">Приведенные ниже примеры относятся к `https://graph.microsoft.com/v1.0`.</span><span class="sxs-lookup"><span data-stu-id="c04e3-121">The following examples are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="c04e3-122">Путь</span><span class="sxs-lookup"><span data-stu-id="c04e3-122">Path</span></span>                                   | <span data-ttu-id="c04e3-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c04e3-123">Description</span></span>
|:---------------------------------------|:------------------------------------
| <span data-ttu-id="c04e3-124">/sites/root</span><span class="sxs-lookup"><span data-stu-id="c04e3-124">/sites/root</span></span>                            | <span data-ttu-id="c04e3-125">Ресурс [site][] по умолчанию для организации.</span><span class="sxs-lookup"><span data-stu-id="c04e3-125">Organization's default [site][].</span></span>
| <span data-ttu-id="c04e3-126">/sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="c04e3-126">/sites/{site-id}</span></span>                       | <span data-ttu-id="c04e3-127">Доступ к определенному ресурсу [site][] с использованием его идентификатора.</span><span class="sxs-lookup"><span data-stu-id="c04e3-127">Access a specific [site][] by its ID.</span></span>
| <span data-ttu-id="c04e3-128">/sites/{site-id}/drive</span><span class="sxs-lookup"><span data-stu-id="c04e3-128">/sites/{site-id}/drive</span></span>                 | <span data-ttu-id="c04e3-129">Доступ к ресурсу [drive](drive.md) (библиотеке документов) для указанного ресурса [site][], заданному по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c04e3-129">Access the default [drive](drive.md) (document library) for the given [site][].</span></span>
| <span data-ttu-id="c04e3-130">/sites/{site-id}/drives</span><span class="sxs-lookup"><span data-stu-id="c04e3-130">/sites/{site-id}/drives</span></span>                | <span data-ttu-id="c04e3-131">Перечисление ресурсов [drive](drive.md) (библиотек документов) для [site][].</span><span class="sxs-lookup"><span data-stu-id="c04e3-131">Enumerate the [drives](drive.md) (document libraries) under the [site][].</span></span>
| <span data-ttu-id="c04e3-132">/sites/{site-id}/sites</span><span class="sxs-lookup"><span data-stu-id="c04e3-132">/sites/{site-id}/sites</span></span>                 | <span data-ttu-id="c04e3-133">Перечисление дочерних сайтов для ресурса [site][].</span><span class="sxs-lookup"><span data-stu-id="c04e3-133">Enumerate the sub-sites under the [site][].</span></span>
| <span data-ttu-id="c04e3-134">/sites/{site-id}/lists</span><span class="sxs-lookup"><span data-stu-id="c04e3-134">/sites/{site-id}/lists</span></span>                 | <span data-ttu-id="c04e3-135">Перечисление ресурсов [lists](list.md) для ресурса [site](site.md).</span><span class="sxs-lookup"><span data-stu-id="c04e3-135">Enumerate the [lists](list.md) under the [site](site.md).</span></span>
| <span data-ttu-id="c04e3-136">/sites/{site-id}/lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="c04e3-136">/sites/{site-id}/lists/{list-id}/items</span></span> | <span data-ttu-id="c04e3-137">Перечисление ресурсов [listItem](listitem.md) для ресурса [list](list.md).</span><span class="sxs-lookup"><span data-stu-id="c04e3-137">Enumerate the [listItems](listitem.md) under the [list](list.md).</span></span>
| <span data-ttu-id="c04e3-138">/groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="c04e3-138">/groups/{group-id}/sites/root</span></span>          | <span data-ttu-id="c04e3-139">Доступ к [сайту][] группы для группы.</span><span class="sxs-lookup"><span data-stu-id="c04e3-139">Access a group's team [site][].</span></span>

<span data-ttu-id="c04e3-p102">К сайту также можно обратиться с помощью соответствующего пути. Для этого укажите имя узла SharePoint, за ним — двоеточие и относительный путь к сайту. При необходимости вы можете менять способ адресации (возвращаться к ресурсной модели), добавляя в конец двоеточие.</span><span class="sxs-lookup"><span data-stu-id="c04e3-p102">Sites can also be addressed by path by using the SharePoint hostname, followed by a colon and the relative path to the site. You can optionally transition back to addressing the resource model by putting another colon at the end.</span></span>

| <span data-ttu-id="c04e3-142">Путь</span><span class="sxs-lookup"><span data-stu-id="c04e3-142">Path</span></span>                                           | <span data-ttu-id="c04e3-143">Описание</span><span class="sxs-lookup"><span data-stu-id="c04e3-143">Description</span></span>
|:-----------------------------------------------|:-----------------------------------
| <span data-ttu-id="c04e3-144">/sites/contoso.sharepoint.com:/teams/hr</span><span class="sxs-lookup"><span data-stu-id="c04e3-144">/sites/contoso.sharepoint.com:/teams/hr</span></span>        | <span data-ttu-id="c04e3-145">Сайт, связанный с https://contoso.sharepoint.com/teams/hr</span><span class="sxs-lookup"><span data-stu-id="c04e3-145">The site associated with https://contoso.sharepoint.com/teams/hr</span></span>
| <span data-ttu-id="c04e3-146">/sites/contoso.sharepoint.com:/teams/hr:/drive</span><span class="sxs-lookup"><span data-stu-id="c04e3-146">/sites/contoso.sharepoint.com:/teams/hr:/drive</span></span> | <span data-ttu-id="c04e3-147">Доступ к ресурсу [drive](drive.md), заданному по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c04e3-147">Access the default [drive](drive.md) for this site.</span></span>

## <a name="note-for-existing-sharepoint-developers"></a><span data-ttu-id="c04e3-148">Примечание, касающееся разработки решений для SharePoint</span><span class="sxs-lookup"><span data-stu-id="c04e3-148">Note for existing SharePoint developers</span></span>

<span data-ttu-id="c04e3-149">API SharePoint в Microsoft Graph имеет ряд ключевых отличий от API CSOM.</span><span class="sxs-lookup"><span data-stu-id="c04e3-149">The Microsoft Graph SharePoint API has a few key differences with the CSOM APIs.</span></span>
<span data-ttu-id="c04e3-150">Ресурс [site][] сопоставляется с `SPWeb`.</span><span class="sxs-lookup"><span data-stu-id="c04e3-150">The [site][] resource maps to `SPWeb`.</span></span>
<span data-ttu-id="c04e3-151">Корневой ресурс [site][] (`SPWeb`) в семействе веб-сайтов имеет аспект [siteCollection](sitecollection.md), содержащий сведения о `SPSite`.</span><span class="sxs-lookup"><span data-stu-id="c04e3-151">The root [site][] (`SPWeb`) in a site collection has a [siteCollection](sitecollection.md) facet, which contains information about the `SPSite`.</span></span>
<span data-ttu-id="c04e3-152">Идентификаторы сайтов уникальны только в пределах одного семейства веб-сайтов. Поэтому чтобы обратиться к сайту по его идентификатору, необходимо указать два идентификатора — для семейства веб-сайтов и для самого сайта.</span><span class="sxs-lookup"><span data-stu-id="c04e3-152">The Microsoft Graph SharePoint API has a few key differences with the CSOM APIs. The site resource maps to . The root site () in a site collection has a siteCollection facet, which contains information about the . Because IDs for sites are only unique within their site collection, addressing a site by ID requires providing both the site collection identifier and the site identifier.</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id},{spweb-id}/
```
<span data-ttu-id="c04e3-153">URL-адрес, содержащий только имя узла, будет указывать на корневой сайт (`SPWeb`) в семействе веб-сайтов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c04e3-153">A URL constructed with only the hostname will point to the root site (`SPWeb`) in the default site collection.</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname}
```

<span data-ttu-id="c04e3-154">URL-адрес, содержащий только имя узла и идентификатор siteCollection (`SPSite`), будет указывать на корневой сайт (`SPWeb`) в указанном семействе веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="c04e3-154">A URL constructed with only the hostname and siteCollection (`SPSite`) ID will point to the root site (`SPWeb`) in the given site collection.</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{hostname},{spsite-id}
```

[site]: site.md
[list]: list.md
[drive]: drive.md
[siteCollection]: siteCollection.md

<!-- {
  "type": "#page.annotation",
  "description": "Getting started programming with the SharePoint API",
  "keywords": "getting started sharepoint rest api programming C# ios android rest http",
  "section": "documentation",
  "tocPath": "Getting Started",
  "tocIndex": -100
} -->
