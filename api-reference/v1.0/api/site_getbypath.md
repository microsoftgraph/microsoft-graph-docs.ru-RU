---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "Получение сайта SharePoint по его пути"
ms.openlocfilehash: 789d4b3f24818a8bc5a06d0c6c14c0002f58f142
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="90e2f-102">Получение ресурса site по его пути</span><span class="sxs-lookup"><span data-stu-id="90e2f-102">Get a site resource by path</span></span>

<span data-ttu-id="90e2f-p101">Получение свойств и отношений ресурса [site][]. Ресурс **site** представляет сайт группы в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="90e2f-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="90e2f-106">Помимо получения ресурса [site по его идентификатору](site_get.md) вы можете получить ресурс site, используя URL-адрес, относительный для сервера.</span><span class="sxs-lookup"><span data-stu-id="90e2f-106">In addition to retrieving a [site by ID](site_get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="90e2f-107">Имя узла семейства веб-сайтов (contoso.sharepoint.com).</span><span class="sxs-lookup"><span data-stu-id="90e2f-107">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="90e2f-108">Путь к сайту, относительный для имени узла сервера.</span><span class="sxs-lookup"><span data-stu-id="90e2f-108">Site path, relative to server hostname.</span></span>

<span data-ttu-id="90e2f-109">Кроме того, существует зарезервированный идентификатор сайта `root`, который всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="90e2f-109">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="90e2f-110">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="90e2f-110">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="90e2f-111">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="90e2f-111">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="90e2f-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90e2f-112">Permissions</span></span>

<span data-ttu-id="90e2f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="90e2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="90e2f-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90e2f-115">Permission type</span></span>      | <span data-ttu-id="90e2f-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90e2f-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90e2f-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90e2f-117">Delegated (work or school account)</span></span> | <span data-ttu-id="90e2f-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90e2f-118">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="90e2f-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90e2f-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90e2f-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90e2f-120">Not supported.</span></span>    |
|<span data-ttu-id="90e2f-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90e2f-121">Application</span></span> | <span data-ttu-id="90e2f-122">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90e2f-122">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90e2f-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90e2f-123">HTTP Request</span></span>

<span data-ttu-id="90e2f-124">Чтобы получить доступ к корневому сайту SharePoint с относительным путем:</span><span class="sxs-lookup"><span data-stu-id="90e2f-124">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="http-response"></a><span data-ttu-id="90e2f-125">HTTP-ответ</span><span class="sxs-lookup"><span data-stu-id="90e2f-125">HTTP Response</span></span>

<span data-ttu-id="90e2f-126">Этот метод возвращает ресурс [site][] для сайта, для ссылки на который используется уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="90e2f-126">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.site" } -->

```http
HTTP/1.1 200 OK

{
  "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
  "owner": {
    "user": { 
      "displayName": "Daron Spektor",
      "id": "5280E7FE-DC7A-4486-9490-E790D81DFEB3"
    }
  },
  "displayName": "OneDrive Team Site",
  "name": "1drvteam",
  "createdDateTime": "2017-05-09T20:56:00Z",
  "lastModifiedDateTime": "2017-05-09T20:56:01Z",
  "webUrl": "https://contoso.sharepoint.com/teams/1drvteam"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by path"
} -->
