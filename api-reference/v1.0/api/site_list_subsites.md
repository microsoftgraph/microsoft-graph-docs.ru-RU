---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "Создание списка дочерних сайтов для сайта SharePoint"
ms.openlocfilehash: a2acf82fca78249e6ea8d05a4a95f88ed741c913
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="enumerate-subsites"></a><span data-ttu-id="67d64-102">Перечисление дочерних сайтов</span><span class="sxs-lookup"><span data-stu-id="67d64-102">Enumerate subsites</span></span>

<span data-ttu-id="67d64-103">Вы можете получить коллекцию дочерних сайтов, определенных для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="67d64-103">Get a collection of subsites defined for a [site][].</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="67d64-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67d64-105">Permissions</span></span>

<span data-ttu-id="67d64-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="67d64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="67d64-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67d64-108">Permission type</span></span>      | <span data-ttu-id="67d64-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67d64-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67d64-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67d64-110">Delegated (work or school account)</span></span> | <span data-ttu-id="67d64-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67d64-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="67d64-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67d64-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67d64-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67d64-113">Not supported.</span></span>    |
|<span data-ttu-id="67d64-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67d64-114">Application</span></span> | <span data-ttu-id="67d64-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67d64-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="67d64-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67d64-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "list-subsites", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/sites
```

## <a name="response"></a><span data-ttu-id="67d64-117">Отклик</span><span class="sxs-lookup"><span data-stu-id="67d64-117">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteA"
    },
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteB"
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/List subsites"
} -->
