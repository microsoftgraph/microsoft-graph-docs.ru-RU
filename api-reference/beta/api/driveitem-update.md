---
author: JeremyKelley
description: Обновление метаданных ресурса DriveItem по идентификатору или пути.
ms.date: 09/10/2017
title: Обновление файла или папки
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 0fa3002a81310b025c51a4ff52930d3b9087c155
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956943"
---
# <a name="update-driveitem-properties"></a><span data-ttu-id="80f91-103">Обновление свойств ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="80f91-103">Update DriveItem properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80f91-104">Обновление метаданных ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути.</span><span class="sxs-lookup"><span data-stu-id="80f91-104">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="80f91-105">Путем обновления также можно [переместить элемент](driveitem-move.md) в другой родительский объект, изменив свойство **parentReference** этого элемента.</span><span class="sxs-lookup"><span data-stu-id="80f91-105">You can also use update to [move an item](driveitem-move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="80f91-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80f91-106">Permissions</span></span>

<span data-ttu-id="80f91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80f91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80f91-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80f91-109">Permission type</span></span>      | <span data-ttu-id="80f91-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80f91-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80f91-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80f91-111">Delegated (work or school account)</span></span> | <span data-ttu-id="80f91-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80f91-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="80f91-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80f91-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80f91-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80f91-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="80f91-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="80f91-115">Application</span></span> | <span data-ttu-id="80f91-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80f91-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80f91-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80f91-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="80f91-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80f91-118">Optional request headers</span></span>

| <span data-ttu-id="80f91-119">Имя</span><span class="sxs-lookup"><span data-stu-id="80f91-119">Name</span></span>          | <span data-ttu-id="80f91-120">Тип</span><span class="sxs-lookup"><span data-stu-id="80f91-120">Type</span></span>   | <span data-ttu-id="80f91-121">Описание</span><span class="sxs-lookup"><span data-stu-id="80f91-121">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="80f91-122">if-match</span><span class="sxs-lookup"><span data-stu-id="80f91-122">if-match</span></span>      | <span data-ttu-id="80f91-123">String</span><span class="sxs-lookup"><span data-stu-id="80f91-123">String</span></span> | <span data-ttu-id="80f91-124">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом eTag папки, то возвращается отклик `412 Precondition Failed`.</span><span class="sxs-lookup"><span data-stu-id="80f91-124">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80f91-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80f91-125">Request body</span></span>

<span data-ttu-id="80f91-126">Укажите в тексте запроса значения обновляемых свойств.</span><span class="sxs-lookup"><span data-stu-id="80f91-126">In the request body, supply the values for properties that should be updated.</span></span>

<span data-ttu-id="80f91-127">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="80f91-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="80f91-128">Для достижения максимальной оптимальной производительности в приложении не следует указывать свойства, которые не были изменены.</span><span class="sxs-lookup"><span data-stu-id="80f91-128">For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="80f91-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="80f91-129">Response</span></span>

<span data-ttu-id="80f91-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="80f91-130">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80f91-131">Пример</span><span class="sxs-lookup"><span data-stu-id="80f91-131">Example</span></span>

<span data-ttu-id="80f91-132">В этом примере показано, как переименовать ресурс DriveItem и присвоить ему имя new-file-name.docx.</span><span class="sxs-lookup"><span data-stu-id="80f91-132">This example renames the DriveItem resource to "new-file-name.docx".</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="80f91-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="80f91-133">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-item" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="80f91-134">C#</span><span class="sxs-lookup"><span data-stu-id="80f91-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="80f91-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="80f91-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="80f91-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="80f91-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="80f91-137">Java</span><span class="sxs-lookup"><span data-stu-id="80f91-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="80f91-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="80f91-138">Response</span></span>

<span data-ttu-id="80f91-139">При успешном выполнении этот метод возвращает ресурс [driveItem][item-resource] в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="80f91-139">If successful, this method returns an [driveItem][item-resource] resource in the response body.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="80f91-140">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="80f91-140">Error responses</span></span>

<span data-ttu-id="80f91-141">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="80f91-141">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of an item.",
  "keywords": "update,replace,contents,item",
  "section": "documentation",
  "tocPath": "Items/Update",
  "suppressions": [
  ]
}
-->
