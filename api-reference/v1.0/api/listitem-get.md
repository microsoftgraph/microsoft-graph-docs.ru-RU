---
author: JeremyKelley
title: Получение ресурса listItem
description: Возвращает метаданные элемента в списке SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 9700f6b18271cc73b0a51d06dc7f8fccdebecb10
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473744"
---
# <a name="get-listitem"></a><span data-ttu-id="96082-103">Получение ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="96082-103">Get listItem</span></span>

<span data-ttu-id="96082-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96082-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="96082-105">Возвращает метаданные [элемента][] в [списке][].</span><span class="sxs-lookup"><span data-stu-id="96082-105">Returns the metadata for an [item][] in a [list][].</span></span>

[списке]: ../resources/list.md
[list]: ../resources/list.md
[элемента]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="96082-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96082-108">Permissions</span></span>

<span data-ttu-id="96082-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96082-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96082-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96082-111">Permission type</span></span>      | <span data-ttu-id="96082-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96082-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96082-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96082-113">Delegated (work or school account)</span></span> | <span data-ttu-id="96082-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96082-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="96082-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96082-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96082-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96082-116">Not supported.</span></span>    |
|<span data-ttu-id="96082-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96082-117">Application</span></span> | <span data-ttu-id="96082-118">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All</span><span class="sxs-lookup"><span data-stu-id="96082-118">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All</span></span> |

> <span data-ttu-id="96082-119">**Примечание.**: Требуется разрешение для приложений Sites.Manage.All, если в списке SharePoint включены параметры утверждения контента.</span><span class="sxs-lookup"><span data-stu-id="96082-119">**Note**: The application permission Sites.Manage.All is required if the SharePoint list has content approval settings turned on.</span></span> <span data-ttu-id="96082-120">В противном случае Microsoft Graph не будет получать элементы списка, которые не имеют состояния «Утверждено».</span><span class="sxs-lookup"><span data-stu-id="96082-120">Otherwise, Microsoft Graph won't retrieve  list items that have an approval status other than Approved.</span></span>

## <a name="http-request"></a><span data-ttu-id="96082-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96082-121">HTTP request</span></span>

<span data-ttu-id="96082-122">Получение ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="96082-122">Get a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
```
<span data-ttu-id="96082-123">Получение значений столбцов ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="96082-123">Get the column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
<span data-ttu-id="96082-124">Получение значений определенных столбцов ресурса listItem</span><span class="sxs-lookup"><span data-stu-id="96082-124">Get specific column values of a listItem</span></span>
```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```
## <a name="optional-query-parameters"></a><span data-ttu-id="96082-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="96082-125">Optional query parameters</span></span>
<span data-ttu-id="96082-126">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="96082-126">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96082-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96082-127">Request headers</span></span>

| <span data-ttu-id="96082-128">Имя</span><span class="sxs-lookup"><span data-stu-id="96082-128">Name</span></span>      |<span data-ttu-id="96082-129">Описание</span><span class="sxs-lookup"><span data-stu-id="96082-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="96082-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96082-130">Authorization</span></span>  | <span data-ttu-id="96082-131">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="96082-131">Bearer {code}.</span></span> <span data-ttu-id="96082-132">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="96082-132">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96082-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96082-133">Request body</span></span>

<span data-ttu-id="96082-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96082-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96082-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="96082-135">Response</span></span> 

<span data-ttu-id="96082-136">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [item][] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="96082-136">If successful, this method returns a `200 OK` response code and an [item][] in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96082-137">Пример</span><span class="sxs-lookup"><span data-stu-id="96082-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="96082-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="96082-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="96082-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="96082-139">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```
# <a name="c"></a>[<span data-ttu-id="96082-140">C#</span><span class="sxs-lookup"><span data-stu-id="96082-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-list-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96082-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96082-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-list-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96082-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96082-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-list-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96082-143">Java</span><span class="sxs-lookup"><span data-stu-id="96082-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-list-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="96082-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="96082-144">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "5",
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
  ]
} -->

