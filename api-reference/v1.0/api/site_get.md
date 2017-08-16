# <a name="get-a-site-resource"></a><span data-ttu-id="f2ce6-101">Получение ресурса site</span><span class="sxs-lookup"><span data-stu-id="f2ce6-101">Get a site resource</span></span>

<span data-ttu-id="f2ce6-p101">Получение свойств и отношений ресурса [site][]. Ресурс **site** представляет сайт группы в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="f2ce6-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

<span data-ttu-id="f2ce6-104">[site]: ../resources/site.md</span><span class="sxs-lookup"><span data-stu-id="f2ce6-104">[site]: ../resources/site.md</span></span>

<span data-ttu-id="f2ce6-105">При обращении ресурс **site** рассматривается как уникальный идентификатор, состоящий из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="f2ce6-105">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="f2ce6-106">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="f2ce6-106">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="f2ce6-107">уникальный идентификатор семейства веб-сайтов (guid);</span><span class="sxs-lookup"><span data-stu-id="f2ce6-107">Site collection unique ID (guid)</span></span>
* <span data-ttu-id="f2ce6-108">уникальный идентификатор сайта (guid).</span><span class="sxs-lookup"><span data-stu-id="f2ce6-108">Site unique ID (guid)</span></span>

<span data-ttu-id="f2ce6-109">Кроме того, существует зарезервированный идентификатор сайта `root`, который всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="f2ce6-109">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="f2ce6-110">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="f2ce6-110">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="f2ce6-111">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="f2ce6-111">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2ce6-112">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f2ce6-112">Prerequisites</span></span>

<span data-ttu-id="f2ce6-113">Для выполнения этого API требуется одно из следующих разрешений:</span><span class="sxs-lookup"><span data-stu-id="f2ce6-113">One of the following scopes is required to execute this request:</span></span>

* <span data-ttu-id="f2ce6-114">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2ce6-114">Sites.Read.All</span></span>
* <span data-ttu-id="f2ce6-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2ce6-115">Sites.ReadWrite.All</span></span>

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="f2ce6-116">Получение корневого сайта клиента</span><span class="sxs-lookup"><span data-stu-id="f2ce6-116">Get the tenant's root site</span></span>

<span data-ttu-id="f2ce6-117">Чтобы получить доступ к корневому сайту SharePoint внутри клиента, создайте следующие запросы:</span><span class="sxs-lookup"><span data-stu-id="f2ce6-117">To access the root SharePoint site within a tenant:</span></span>

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="f2ce6-118">Использование относительного URL-адреса сервера для доступа к сайту</span><span class="sxs-lookup"><span data-stu-id="f2ce6-118">Access a site by server-relative URL</span></span>

<span data-ttu-id="f2ce6-119">Если у вас есть относительный URL-адрес сервера для ресурса **site**, можно создать следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="f2ce6-119">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="f2ce6-120">Доступ к сайту группы для ресурса group</span><span class="sxs-lookup"><span data-stu-id="f2ce6-120">Access a group team site</span></span>

<span data-ttu-id="f2ce6-121">Чтобы получить доступ к сайту группы для ресурса [group](../resources/group.md), создайте следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="f2ce6-121">To access the team site for a [group](../resources/group.md):</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="f2ce6-122">Пример</span><span class="sxs-lookup"><span data-stu-id="f2ce6-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f2ce6-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2ce6-123">Request</span></span>

<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}
```

##### <a name="response"></a><span data-ttu-id="f2ce6-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2ce6-124">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "d297964f-d325-424b-a002-f54048a4622e",
    "name": "OneDrive / SharePoint Team",
    "description": "Collaboration site for the OneDrive and SharePoint team",
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/Get site by ID"
} -->
