---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Создание списка списков SharePoint на сайте
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5eaa02bad7ce4997386a6b113bf7854493a67e90
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880316"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="9ee66-102">Перечисление списков на сайте</span><span class="sxs-lookup"><span data-stu-id="9ee66-102">Enumerate lists in a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ee66-103">Получение коллекции [списков][] для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="9ee66-103">Get the collection of [lists][] for a [site][].</span></span>

[списков]: ../resources/list.md
[lists]: ../resources/list.md
[сайта]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="9ee66-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ee66-106">Permissions</span></span>

<span data-ttu-id="9ee66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ee66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ee66-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ee66-109">Permission type</span></span>      | <span data-ttu-id="9ee66-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ee66-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ee66-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ee66-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9ee66-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ee66-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9ee66-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ee66-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ee66-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ee66-114">Not supported.</span></span>    |
|<span data-ttu-id="9ee66-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ee66-115">Application</span></span> | <span data-ttu-id="9ee66-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ee66-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ee66-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ee66-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="9ee66-118">Пример</span><span class="sxs-lookup"><span data-stu-id="9ee66-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9ee66-119">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ee66-119">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9ee66-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ee66-120">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ee66-121">C#</span><span class="sxs-lookup"><span data-stu-id="9ee66-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ee66-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="9ee66-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ee66-123">Цель — C</span><span class="sxs-lookup"><span data-stu-id="9ee66-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9ee66-124">Java</span><span class="sxs-lookup"><span data-stu-id="9ee66-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9ee66-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ee66-125">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b57af081-936c-4803-a120-d94887b03864",
      "name": "Documents",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "documentLibrary"
       }
    },
    {
      "id": "1234-112-112-4",
      "name": "MicroFeed",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "genericList"
       }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="9ee66-126">Заметки</span><span class="sxs-lookup"><span data-stu-id="9ee66-126">Remarks</span></span>

<span data-ttu-id="9ee66-127">По умолчанию ресурсы list с аспектом [system][] скрыты.</span><span class="sxs-lookup"><span data-stu-id="9ee66-127">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="9ee66-128">Чтобы перечислить их, включите `system` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="9ee66-128">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate",
  "suppressions": [
  ]
}
-->
