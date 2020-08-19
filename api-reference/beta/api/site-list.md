---
title: Перечисление сайтов
description: Перечислите доступные [сайты] [] в Организации, которые совпадают с предоставленными критериями фильтра и параметрами запроса.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: JeremyKelley
ms.openlocfilehash: bfedee99e7679aead910c675d605c0f0b776d42b
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809889"
---
# <a name="enumerate-sites"></a><span data-ttu-id="a4b72-103">Перечисление сайтов</span><span class="sxs-lookup"><span data-stu-id="a4b72-103">Enumerate sites</span></span>

<span data-ttu-id="a4b72-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4b72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4b72-105">Список доступных [сайтов][] в Организации, которые отвечают предоставленным условиям фильтра и параметрам запроса.</span><span class="sxs-lookup"><span data-stu-id="a4b72-105">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="a4b72-106">В настоящее время поддерживаются только следующие параметры запросов:</span><span class="sxs-lookup"><span data-stu-id="a4b72-106">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="a4b72-107">Оператор Filter</span><span class="sxs-lookup"><span data-stu-id="a4b72-107">Filter statement</span></span>             | <span data-ttu-id="a4b72-108">Оператор SELECT</span><span class="sxs-lookup"><span data-stu-id="a4b72-108">Select statement</span></span>        | <span data-ttu-id="a4b72-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a4b72-109">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="a4b72-110">Перечисление всех семейств сайтов корневого уровня в Организации.</span><span class="sxs-lookup"><span data-stu-id="a4b72-110">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="a4b72-111">Полезен для обнаружения домашнего сайта для каждого из географических регионов.</span><span class="sxs-lookup"><span data-stu-id="a4b72-111">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="a4b72-112">Кроме того, вы можете использовать **[$searchный][]** запрос для поиска сайтов, отвечающих заданному ключевому слову.</span><span class="sxs-lookup"><span data-stu-id="a4b72-112">In addition, you may use a **[$search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[$search]: site-search.md
[сайтов]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="a4b72-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4b72-115">Permissions</span></span>

<span data-ttu-id="a4b72-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4b72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4b72-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4b72-118">Permission type</span></span>                        | <span data-ttu-id="a4b72-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4b72-119">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="a4b72-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4b72-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="a4b72-121">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4b72-121">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="a4b72-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4b72-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4b72-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4b72-123">Not supported.</span></span>
|<span data-ttu-id="a4b72-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4b72-124">Application</span></span>                            | <span data-ttu-id="a4b72-125">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4b72-125">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="a4b72-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4b72-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites?$filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="a4b72-127">Пример</span><span class="sxs-lookup"><span data-stu-id="a4b72-127">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a4b72-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4b72-128">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a4b72-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4b72-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-sites" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites?$select=siteCollection,webUrl&$filter=siteCollection/root%20ne%20null
```
# <a name="c"></a>[<span data-ttu-id="a4b72-130">C#</span><span class="sxs-lookup"><span data-stu-id="a4b72-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4b72-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4b72-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4b72-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4b72-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a4b72-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4b72-133">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
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
