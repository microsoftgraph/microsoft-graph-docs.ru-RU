---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Обновление файла или папки
localization_priority: Priority
ms.prod: sharepoint
description: Обновление метаданных ресурса DriveItem по идентификатору или пути.
doc_type: apiPageType
ms.openlocfilehash: 799a643170a89336fe24d3e7bc4922e6bd007ff4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063794"
---
# <a name="update-driveitem-properties"></a><span data-ttu-id="a32e8-103">Обновление свойств ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="a32e8-103">Update DriveItem properties</span></span>

<span data-ttu-id="a32e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a32e8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a32e8-105">Обновление метаданных ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути.</span><span class="sxs-lookup"><span data-stu-id="a32e8-105">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="a32e8-106">Путем обновления также можно [переместить элемент](driveitem-move.md) в другой родительский объект, изменив свойство **parentReference** этого элемента.</span><span class="sxs-lookup"><span data-stu-id="a32e8-106">You can also use update to [move an item](driveitem-move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="a32e8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a32e8-107">Permissions</span></span>

<span data-ttu-id="a32e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a32e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a32e8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a32e8-110">Permission type</span></span>      | <span data-ttu-id="a32e8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a32e8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a32e8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a32e8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a32e8-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a32e8-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a32e8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a32e8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a32e8-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a32e8-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a32e8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a32e8-116">Application</span></span> | <span data-ttu-id="a32e8-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a32e8-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a32e8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a32e8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="a32e8-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a32e8-119">Optional request headers</span></span>

| <span data-ttu-id="a32e8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a32e8-120">Name</span></span>          | <span data-ttu-id="a32e8-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a32e8-121">Type</span></span>   | <span data-ttu-id="a32e8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a32e8-122">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a32e8-123">if-match</span><span class="sxs-lookup"><span data-stu-id="a32e8-123">if-match</span></span>      | <span data-ttu-id="a32e8-124">String</span><span class="sxs-lookup"><span data-stu-id="a32e8-124">String</span></span> | <span data-ttu-id="a32e8-125">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом eTag папки, то возвращается отклик `412 Precondition Failed`.</span><span class="sxs-lookup"><span data-stu-id="a32e8-125">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a32e8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a32e8-126">Request body</span></span>

<span data-ttu-id="a32e8-127">Укажите в тексте запроса значения обновляемых свойств.</span><span class="sxs-lookup"><span data-stu-id="a32e8-127">In the request body, supply the values for properties that should be updated.</span></span>

<span data-ttu-id="a32e8-128">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="a32e8-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="a32e8-129">Для достижения максимальной оптимальной производительности в приложении не следует указывать свойства, которые не были изменены.</span><span class="sxs-lookup"><span data-stu-id="a32e8-129">For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="a32e8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a32e8-130">Response</span></span>

<span data-ttu-id="a32e8-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a32e8-131">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a32e8-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a32e8-132">Example</span></span>

<span data-ttu-id="a32e8-133">В этом примере показано, как переименовать ресурс DriveItem и присвоить ему имя new-file-name.docx.</span><span class="sxs-lookup"><span data-stu-id="a32e8-133">This example renames the DriveItem resource to "new-file-name.docx".</span></span>


# <a name="http"></a>[<span data-ttu-id="a32e8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a32e8-134">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-item", "tags": "service.graph" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```
# <a name="c"></a>[<span data-ttu-id="a32e8-135">C#</span><span class="sxs-lookup"><span data-stu-id="a32e8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a32e8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a32e8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a32e8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a32e8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a32e8-138">Java</span><span class="sxs-lookup"><span data-stu-id="a32e8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a32e8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a32e8-139">Response</span></span>

<span data-ttu-id="a32e8-140">При успешном выполнении этот метод возвращает ресурс [driveItem][item-resource] в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a32e8-140">If successful, this method returns an [driveItem][item-resource] resource in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "name": "new-file-name.docx",
  "file": { }
}
```

## <a name="error-responses"></a><span data-ttu-id="a32e8-141">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="a32e8-141">Error responses</span></span>

<span data-ttu-id="a32e8-142">Дополнительные сведения о возвращении ошибок см. в статье [Ответы с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="a32e8-142">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of an item.",
  "keywords": "update,replace,contents,item",
  "section": "documentation",
  "tocPath": "Items/Update",
  "suppressions": [
  ]
} -->

