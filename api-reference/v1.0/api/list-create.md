---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Создание списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
description: Создание списка на сайте.
doc_type: apiPageType
ms.openlocfilehash: 96ab4b1f80ea85a6c17c7ad1d22214dac4bf687e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038468"
---
# <a name="create-a-new-list"></a><span data-ttu-id="0bb44-103">Создание списка</span><span class="sxs-lookup"><span data-stu-id="0bb44-103">Create a new list</span></span>

<span data-ttu-id="0bb44-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bb44-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0bb44-105">Создание [списка][] на [сайте][].</span><span class="sxs-lookup"><span data-stu-id="0bb44-105">Create a new [list][] in a [site][].</span></span>

## <a name="permissions"></a><span data-ttu-id="0bb44-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0bb44-106">Permissions</span></span>

<span data-ttu-id="0bb44-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bb44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="0bb44-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0bb44-109">Permission type</span></span>             | <span data-ttu-id="0bb44-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0bb44-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="0bb44-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0bb44-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0bb44-112">Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="0bb44-112">Sites.Manage.All</span></span>                            |
| <span data-ttu-id="0bb44-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0bb44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bb44-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bb44-114">Not supported.</span></span>                              |
| <span data-ttu-id="0bb44-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0bb44-115">Application</span></span>                            | <span data-ttu-id="0bb44-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bb44-116">Sites.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0bb44-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0bb44-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="request-body"></a><span data-ttu-id="0bb44-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0bb44-118">Request body</span></span>

<span data-ttu-id="0bb44-119">В теле запроса укажите представление ресурса [списка][], который необходимо создать, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0bb44-119">In the request body, supply a JSON representation of the [list][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="0bb44-120">Пример</span><span class="sxs-lookup"><span data-stu-id="0bb44-120">Example</span></span>

<span data-ttu-id="0bb44-121">В примере ниже показано, как создать список общего назначения.</span><span class="sxs-lookup"><span data-stu-id="0bb44-121">Here is an example of how to create a new generic list.</span></span>


# <a name="http"></a>[<span data-ttu-id="0bb44-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="0bb44-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-list", "scopes": "sites.readwrite.all" } -->

```http
POST /sites/{site-id}/lists
Content-Type: application/json

{
  "displayName": "Books",
  "columns": [
    {
      "name": "Author",
      "text": { }
    },
    {
      "name": "PageCount",
      "number": { }
    }
  ],
  "list": {
    "template": "genericList"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="0bb44-123">C#</span><span class="sxs-lookup"><span data-stu-id="0bb44-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0bb44-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0bb44-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0bb44-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0bb44-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0bb44-126">Java</span><span class="sxs-lookup"><span data-stu-id="0bb44-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="0bb44-127">**Примечание.** Настраиваемые столбцы являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="0bb44-127">**Note:** Custom columns are optional.</span></span>

<span data-ttu-id="0bb44-128">Помимо столбцов, указанных здесь, в создаваемых списках используются столбцы, заданные в соответствующем **шаблоне**.</span><span class="sxs-lookup"><span data-stu-id="0bb44-128">In addition to any columns specified here, new lists are created with columns defined in the referenced **template**.</span></span>
<span data-ttu-id="0bb44-129">Если аспект или **шаблон** **списка** не указаны, то по умолчанию для списка используется шаблон `genericList`, включающий столбец _Title_ (Название).</span><span class="sxs-lookup"><span data-stu-id="0bb44-129">If the **list** facet or **template** is unspecified, the list defaults to the `genericList` template, which includes a _Title_ column.</span></span>

## <a name="response"></a><span data-ttu-id="0bb44-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="0bb44-130">Response</span></span>

<span data-ttu-id="0bb44-131">При успешном выполнении этот метод возвращает объект [списка][] для вновь созданного списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0bb44-131">If successful, this method returns a [list][] in the response body for the created list.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.list", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "22e03ef3-6ef4-424d-a1d3-92a337807c30",
  "createdDateTime": "2017-04-30T01:21:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```

<span data-ttu-id="0bb44-132">**Примечание.** Ответ усечен для наглядности.</span><span class="sxs-lookup"><span data-stu-id="0bb44-132">**Note:** The response object is truncated for clarity.</span></span>
<span data-ttu-id="0bb44-133">При фактическом вызове будут возвращены свойства, используемые по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0bb44-133">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[site]: ../resources/site.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a new SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "List/Create",
  "suppressions": [
  ]
} -->

