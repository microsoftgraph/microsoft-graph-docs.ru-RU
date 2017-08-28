# <a name="get-a-site-resource"></a><span data-ttu-id="7c85d-101">Получение ресурса site</span><span class="sxs-lookup"><span data-stu-id="7c85d-101">Get a site resource</span></span>

<span data-ttu-id="7c85d-p101">Получение свойств и отношений ресурса [site][]. Ресурс **site** представляет сайт группы в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7c85d-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

<span data-ttu-id="7c85d-104">[site]: ../resources/site.md</span><span class="sxs-lookup"><span data-stu-id="7c85d-104">[site]: ../resources/site.md</span></span>

<span data-ttu-id="7c85d-105">При обращении ресурс **site** рассматривается как уникальный идентификатор, состоящий из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="7c85d-105">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="7c85d-106">имя узла семейства веб-сайтов (contoso.sharepoint.com);</span><span class="sxs-lookup"><span data-stu-id="7c85d-106">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="7c85d-107">уникальный идентификатор семейства веб-сайтов (guid);</span><span class="sxs-lookup"><span data-stu-id="7c85d-107">Site collection unique ID (guid)</span></span>
* <span data-ttu-id="7c85d-108">уникальный идентификатор сайта (guid).</span><span class="sxs-lookup"><span data-stu-id="7c85d-108">Site unique ID (guid)</span></span>

<span data-ttu-id="7c85d-109">Кроме того, существует зарезервированный идентификатор сайта `root`, который всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="7c85d-109">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="7c85d-110">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="7c85d-110">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="7c85d-111">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="7c85d-111">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c85d-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c85d-112">Permissions</span></span>

<span data-ttu-id="7c85d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c85d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7c85d-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c85d-115">Permission type</span></span>      | <span data-ttu-id="7c85d-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c85d-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c85d-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c85d-117">Delegated (work or school account)</span></span> | <span data-ttu-id="7c85d-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c85d-118">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7c85d-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c85d-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c85d-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c85d-120">Not supported.</span></span>    |
|<span data-ttu-id="7c85d-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c85d-121">Application</span></span> | <span data-ttu-id="7c85d-122">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c85d-122">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="7c85d-123">Получение корневого сайта клиента</span><span class="sxs-lookup"><span data-stu-id="7c85d-123">Get the tenant's root site</span></span>

<span data-ttu-id="7c85d-124">Чтобы получить доступ к корневому сайту SharePoint внутри клиента, создайте следующие запросы:</span><span class="sxs-lookup"><span data-stu-id="7c85d-124">To access the root SharePoint site within a tenant:</span></span>

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="7c85d-125">Использование относительного URL-адреса сервера для доступа к сайту</span><span class="sxs-lookup"><span data-stu-id="7c85d-125">Access a site by server-relative URL</span></span>

<span data-ttu-id="7c85d-126">Если у вас есть относительный URL-адрес сервера для ресурса **site**, можно создать следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="7c85d-126">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="7c85d-127">Доступ к сайту группы для ресурса group</span><span class="sxs-lookup"><span data-stu-id="7c85d-127">Access a group team site</span></span>

<span data-ttu-id="7c85d-128">Чтобы получить доступ к сайту группы для ресурса [group](../resources/group.md), создайте следующий запрос:</span><span class="sxs-lookup"><span data-stu-id="7c85d-128">To access the team site for a [group](../resources/group.md):</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="7c85d-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7c85d-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7c85d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c85d-130">Request</span></span>

<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}
```

##### <a name="response"></a><span data-ttu-id="7c85d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c85d-131">Response</span></span>

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
