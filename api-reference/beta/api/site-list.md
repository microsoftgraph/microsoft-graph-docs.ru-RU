---
title: Перечисление сайтов
description: Список [] доступных [сайтов] в организации, соответствующих указанным критериям фильтра и запроса.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 05c3480181126d528657d0efacde97051a178bfd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939569"
---
# <a name="enumerate-sites"></a><span data-ttu-id="44a15-103">Перечисление сайтов</span><span class="sxs-lookup"><span data-stu-id="44a15-103">Enumerate sites</span></span>

> <span data-ttu-id="44a15-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="44a15-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44a15-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44a15-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44a15-106">Список доступных [сайтов][] в организации, которая соответствуют указанным отбора и запроса.</span><span class="sxs-lookup"><span data-stu-id="44a15-106">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="44a15-107">В настоящее время поддерживаются только следующие параметры запроса:</span><span class="sxs-lookup"><span data-stu-id="44a15-107">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="44a15-108">Оператор фильтра</span><span class="sxs-lookup"><span data-stu-id="44a15-108">Filter statement</span></span>             | <span data-ttu-id="44a15-109">Оператор SELECT</span><span class="sxs-lookup"><span data-stu-id="44a15-109">Select statement</span></span>        | <span data-ttu-id="44a15-110">Описание</span><span class="sxs-lookup"><span data-stu-id="44a15-110">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="44a15-111">Список всех семейств сайтов корневого уровня в организации.</span><span class="sxs-lookup"><span data-stu-id="44a15-111">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="44a15-112">Полезные при обнаружении главного сайта для каждого География.</span><span class="sxs-lookup"><span data-stu-id="44a15-112">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="44a15-113">Кроме того могут используйте запрос **[поиска][]** семейства сайтов «/ sites» для поиска сайты, соответствующие заданным ключевые слова.</span><span class="sxs-lookup"><span data-stu-id="44a15-113">In addition, you may use a **[search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[Поиск]: site-search.md
[search]: site-search.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="44a15-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44a15-116">Permissions</span></span>

<span data-ttu-id="44a15-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44a15-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44a15-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44a15-119">Permission type</span></span>                        | <span data-ttu-id="44a15-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44a15-120">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="44a15-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44a15-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="44a15-122">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44a15-122">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="44a15-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44a15-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44a15-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44a15-124">Not supported.</span></span>
|<span data-ttu-id="44a15-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44a15-125">Application</span></span>                            | <span data-ttu-id="44a15-126">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44a15-126">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="44a15-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44a15-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="44a15-128">Пример</span><span class="sxs-lookup"><span data-stu-id="44a15-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="44a15-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="44a15-129">Request</span></span>

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a><span data-ttu-id="44a15-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="44a15-130">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites"
} -->
