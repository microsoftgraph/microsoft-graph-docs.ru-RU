---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Получение сайта SharePoint по его пути
ms.openlocfilehash: 7d63fd3651ab870318af46a298d6b945f331eda8
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748278"
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="fe3e2-102">Получение ресурса site по его пути</span><span class="sxs-lookup"><span data-stu-id="fe3e2-102">Get a site resource by path</span></span>

> <span data-ttu-id="fe3e2-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fe3e2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe3e2-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe3e2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe3e2-p102">Получение свойств и отношений ресурса [site][]. Ресурс **site** представляет сайт группы в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fe3e2-p102">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="fe3e2-108">Помимо получения ресурса [site по его идентификатору](site-get.md) вы можете получить ресурс site, используя URL-адрес, относительный для сервера.</span><span class="sxs-lookup"><span data-stu-id="fe3e2-108">In addition to retrieving a [site by ID](site-get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="fe3e2-109">Имя узла семейства веб-сайтов (contoso.sharepoint.com).</span><span class="sxs-lookup"><span data-stu-id="fe3e2-109">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="fe3e2-110">Путь к сайту, относительный для имени узла сервера.</span><span class="sxs-lookup"><span data-stu-id="fe3e2-110">Site path, relative to server hostname.</span></span>

<span data-ttu-id="fe3e2-111">Кроме того, существует зарезервированный идентификатор сайта `root`, который всегда ссылается на корневой сайт указанного целевого объекта, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="fe3e2-111">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="fe3e2-112">`/sites/root`. Корневой сайт клиента.</span><span class="sxs-lookup"><span data-stu-id="fe3e2-112">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="fe3e2-113">`/groups/{group-id}/sites/root`. Сайт группы для ресурса group.</span><span class="sxs-lookup"><span data-stu-id="fe3e2-113">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe3e2-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe3e2-114">Permissions</span></span>

<span data-ttu-id="fe3e2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe3e2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe3e2-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe3e2-117">Permission type</span></span>      | <span data-ttu-id="fe3e2-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe3e2-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe3e2-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe3e2-119">Delegated (work or school account)</span></span> | <span data-ttu-id="fe3e2-120">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe3e2-120">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe3e2-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe3e2-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe3e2-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe3e2-122">Not supported.</span></span>    |
|<span data-ttu-id="fe3e2-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe3e2-123">Application</span></span> | <span data-ttu-id="fe3e2-124">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe3e2-124">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe3e2-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe3e2-125">HTTP Request</span></span>

<span data-ttu-id="fe3e2-126">Чтобы получить доступ к корневому сайту SharePoint с использованием относительного пути, выполните указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="fe3e2-126">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a><span data-ttu-id="fe3e2-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe3e2-127">Response</span></span>

<span data-ttu-id="fe3e2-128">Этот метод возвращает ресурс [site][] для сайта, для ссылки на который используется уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="fe3e2-128">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

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
