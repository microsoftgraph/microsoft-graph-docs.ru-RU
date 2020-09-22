---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Создание записи в списке SharePoint
localization_priority: Priority
ms.prod: sharepoint
description: Создание ресурса listItem в списке.
doc_type: apiPageType
ms.openlocfilehash: 1a51af48b8349eb0b505b7ded88721caa53bb68c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057341"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="9e956-103">Создание элемента в списке</span><span class="sxs-lookup"><span data-stu-id="9e956-103">Create a new item in a list</span></span>

<span data-ttu-id="9e956-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e956-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e956-105">Создание элемента [listItem][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="9e956-105">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="9e956-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e956-106">Permissions</span></span>

<span data-ttu-id="9e956-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e956-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e956-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e956-109">Permission type</span></span>      | <span data-ttu-id="9e956-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e956-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e956-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e956-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9e956-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e956-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9e956-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e956-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e956-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e956-114">Not supported.</span></span>    |
|<span data-ttu-id="9e956-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e956-115">Application</span></span> | <span data-ttu-id="9e956-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e956-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e956-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e956-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="9e956-118">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9e956-118">Request body</span></span>

<span data-ttu-id="9e956-119">В теле запроса укажите представление ресурса [listItem][], который необходимо создать, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e956-119">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="9e956-120">Пример</span><span class="sxs-lookup"><span data-stu-id="9e956-120">Example</span></span>

<span data-ttu-id="9e956-121">В примере ниже показано, как создать элемент списка общего назначения.</span><span class="sxs-lookup"><span data-stu-id="9e956-121">Here is an example of how to create a new generic list item.</span></span>


# <a name="http"></a>[<span data-ttu-id="9e956-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e956-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
Content-Type: application/json

{
  "fields": {
    "Title": "Widget",
    "Color": "Purple",
    "Weight": 32
  }
}
```
# <a name="c"></a>[<span data-ttu-id="9e956-123">C#</span><span class="sxs-lookup"><span data-stu-id="9e956-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-listitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e956-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e956-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-listitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e956-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e956-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-listitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9e956-126">Java</span><span class="sxs-lookup"><span data-stu-id="9e956-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-listitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="9e956-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e956-127">Response</span></span>

<span data-ttu-id="9e956-128">При успешном выполнении этот метод возвращает объект [listItem][] для созданного элемента списка в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9e956-128">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "20",
  "createdDateTime": "2016-08-30T08:26:00Z",
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

<span data-ttu-id="9e956-129">**Примечание.** Ответ усечен для наглядности.</span><span class="sxs-lookup"><span data-stu-id="9e956-129">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="9e956-130">При фактическом вызове будут возвращены свойства, используемые по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9e956-130">Default properties will be returned from the actual call.</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[listItem]: ../resources/listitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create",
  "suppressions": [
  ]
} -->

