---
title: ПереЧисление сайтов
description: ПереЧислите доступные [сайты] [] в Организации, которые совпадают с предоставленными критериями фильтра и параметрами запроса.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f225d9990637f8251ae40e3f66b0f993bbf74f32
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545207"
---
# <a name="enumerate-sites"></a><span data-ttu-id="01245-103">ПереЧисление сайтов</span><span class="sxs-lookup"><span data-stu-id="01245-103">Enumerate sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01245-104">Список доступных [сайтов][] в Организации, которые отвечают предоставленным условиям фильтра и параметрам запроса.</span><span class="sxs-lookup"><span data-stu-id="01245-104">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="01245-105">В настоящее время поддерживаются только следующие параметры запросов:</span><span class="sxs-lookup"><span data-stu-id="01245-105">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="01245-106">Оператор Filter</span><span class="sxs-lookup"><span data-stu-id="01245-106">Filter statement</span></span>             | <span data-ttu-id="01245-107">Оператор SELECT</span><span class="sxs-lookup"><span data-stu-id="01245-107">Select statement</span></span>        | <span data-ttu-id="01245-108">Описание</span><span class="sxs-lookup"><span data-stu-id="01245-108">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="01245-109">ПереЧисление всех семейств сайтов корневого уровня в Организации.</span><span class="sxs-lookup"><span data-stu-id="01245-109">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="01245-110">Полезен для обнаружения домашнего сайта для каждого из географических регионов.</span><span class="sxs-lookup"><span data-stu-id="01245-110">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="01245-111">Кроме того, вы можете использовать **[поисковый][]** запрос в семействе "" "" "" "" "" "" "" "" "" "" "</span><span class="sxs-lookup"><span data-stu-id="01245-111">In addition, you may use a **[search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[выполнять]: site-search.md
[search]: site-search.md
[сайтов]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="01245-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01245-114">Permissions</span></span>

<span data-ttu-id="01245-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01245-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01245-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01245-117">Permission type</span></span>                        | <span data-ttu-id="01245-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01245-118">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="01245-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01245-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="01245-120">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01245-120">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="01245-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01245-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01245-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01245-122">Not supported.</span></span>
|<span data-ttu-id="01245-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01245-123">Application</span></span>                            | <span data-ttu-id="01245-124">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01245-124">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="01245-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01245-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="01245-126">Пример</span><span class="sxs-lookup"><span data-stu-id="01245-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="01245-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="01245-127">Request</span></span>

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a><span data-ttu-id="01245-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="01245-128">Response</span></span>

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
    "Error: /api-reference/beta/api/site-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
