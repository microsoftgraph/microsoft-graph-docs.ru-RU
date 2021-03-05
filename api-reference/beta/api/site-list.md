---
title: Переумерия сайтов
description: Список доступных [сайтов][] в организации, которая соответствует критериям фильтра и параметрам запроса.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: JeremyKelley
ms.openlocfilehash: c1b8af50227346e4440e4ca98873b20160ecd81b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475786"
---
# <a name="enumerate-sites"></a><span data-ttu-id="7f7b5-103">Переумерия сайтов</span><span class="sxs-lookup"><span data-stu-id="7f7b5-103">Enumerate sites</span></span>

<span data-ttu-id="7f7b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f7b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f7b5-105">Список доступных [сайтов в][] организации, которая соответствует предоставленным критериям фильтрации и параметрам запроса.</span><span class="sxs-lookup"><span data-stu-id="7f7b5-105">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="7f7b5-106">В настоящее время поддерживаются только следующие параметры запроса:</span><span class="sxs-lookup"><span data-stu-id="7f7b5-106">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="7f7b5-107">Заявление фильтра</span><span class="sxs-lookup"><span data-stu-id="7f7b5-107">Filter statement</span></span>             | <span data-ttu-id="7f7b5-108">Выберите утверждение</span><span class="sxs-lookup"><span data-stu-id="7f7b5-108">Select statement</span></span>        | <span data-ttu-id="7f7b5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7f7b5-109">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="7f7b5-110">Списки всех корневых коллекций сайтов в организации.</span><span class="sxs-lookup"><span data-stu-id="7f7b5-110">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="7f7b5-111">Полезно для обнаружения домашнего сайта для каждой географии.</span><span class="sxs-lookup"><span data-stu-id="7f7b5-111">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="7f7b5-112">Кроме того, для поиска сайтов, **[совпадающих с ключевыми словами,][]** можно использовать $search запрос в отношении коллекции "/сайты".</span><span class="sxs-lookup"><span data-stu-id="7f7b5-112">In addition, you may use a **[$search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[$search]: site-search.md
[сайтов]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="7f7b5-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f7b5-115">Permissions</span></span>

<span data-ttu-id="7f7b5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f7b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f7b5-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f7b5-118">Permission type</span></span>                        | <span data-ttu-id="7f7b5-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f7b5-119">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="7f7b5-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f7b5-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f7b5-121">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f7b5-121">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="7f7b5-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f7b5-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f7b5-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f7b5-123">Not supported.</span></span>
|<span data-ttu-id="7f7b5-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f7b5-124">Application</span></span>                            | <span data-ttu-id="7f7b5-125">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f7b5-125">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="7f7b5-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f7b5-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites?$filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="7f7b5-127">Пример</span><span class="sxs-lookup"><span data-stu-id="7f7b5-127">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7f7b5-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f7b5-128">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7f7b5-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f7b5-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-sites" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites?$select=siteCollection,webUrl&$filter=siteCollection/root%20ne%20null
```
# <a name="c"></a>[<span data-ttu-id="7f7b5-130">C#</span><span class="sxs-lookup"><span data-stu-id="7f7b5-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f7b5-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f7b5-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f7b5-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f7b5-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f7b5-133">Java</span><span class="sxs-lookup"><span data-stu-id="7f7b5-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-sites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7f7b5-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f7b5-134">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Contoso USA",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com",
        "dataLocationCode": "NAM",
        "root": { }
      },
      "webUrl": "https://contoso.sharepoint.com"
    },
    {
      "id": "contoso-jpn.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Contoso Japan",
      "root": { },
      "siteCollection": {
        "hostname": "contoso-jp.sharepoint.com",
        "dataLocationCode": "JPN",
        "root": { }
      },
      "webUrl": "https://contoso-jp.sharepoint.com"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
  ]
}
-->


