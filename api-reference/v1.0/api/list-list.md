---
author: JeremyKelley
ms.date: 09/11/2017
title: Создание списка списков SharePoint на сайте
localization_priority: Priority
ms.prod: sharepoint
description: Получение коллекции списков для сайта.
doc_type: apiPageType
ms.openlocfilehash: ce7cd7807093a190cae007eb70445ea5de7bb0e7
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473765"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="41dc9-103">Перечисление списков на сайте</span><span class="sxs-lookup"><span data-stu-id="41dc9-103">Enumerate lists in a site</span></span>

<span data-ttu-id="41dc9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41dc9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41dc9-105">Получение коллекции [списков][] для [сайта][].</span><span class="sxs-lookup"><span data-stu-id="41dc9-105">Get the collection of [lists][] for a [site][].</span></span>

[списков]: ../resources/list.md
[lists]: ../resources/list.md
[сайта]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="41dc9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41dc9-108">Permissions</span></span>

<span data-ttu-id="41dc9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41dc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41dc9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41dc9-111">Permission type</span></span>      | <span data-ttu-id="41dc9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41dc9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41dc9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41dc9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="41dc9-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41dc9-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="41dc9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41dc9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41dc9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41dc9-116">Not supported.</span></span>    |
|<span data-ttu-id="41dc9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41dc9-117">Application</span></span> | <span data-ttu-id="41dc9-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41dc9-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41dc9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41dc9-119">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="41dc9-120">Пример</span><span class="sxs-lookup"><span data-stu-id="41dc9-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="41dc9-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="41dc9-121">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="41dc9-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="41dc9-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```
# <a name="c"></a>[<span data-ttu-id="41dc9-123">C#</span><span class="sxs-lookup"><span data-stu-id="41dc9-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41dc9-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41dc9-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41dc9-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41dc9-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41dc9-126">Java</span><span class="sxs-lookup"><span data-stu-id="41dc9-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="41dc9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="41dc9-127">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "isCollection": true, "truncated": true } -->

```http
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

## <a name="remarks"></a><span data-ttu-id="41dc9-128">Заметки</span><span class="sxs-lookup"><span data-stu-id="41dc9-128">Remarks</span></span>

<span data-ttu-id="41dc9-129">По умолчанию ресурсы list с аспектом [system][] скрыты.</span><span class="sxs-lookup"><span data-stu-id="41dc9-129">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="41dc9-130">Чтобы перечислить их, включите `system` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="41dc9-130">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate",
  "suppressions": [
  ]
} -->

