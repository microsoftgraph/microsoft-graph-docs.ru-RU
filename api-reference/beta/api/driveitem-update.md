---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Обновление файла или папки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3eb23e5657794a4ef4062cc8b36cc003055e38c2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260006"
---
# <a name="update-driveitem-properties"></a><span data-ttu-id="a0956-102">Обновление свойств ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="a0956-102">Update DriveItem properties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0956-103">Обновление метаданных ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути.</span><span class="sxs-lookup"><span data-stu-id="a0956-103">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="a0956-104">Путем обновления также можно [переместить элемент](driveitem-move.md) в другой родительский объект, изменив свойство **parentReference** этого элемента.</span><span class="sxs-lookup"><span data-stu-id="a0956-104">You can also use update to [move an item](driveitem-move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0956-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0956-105">Permissions</span></span>

<span data-ttu-id="a0956-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0956-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0956-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0956-108">Permission type</span></span>      | <span data-ttu-id="a0956-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0956-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0956-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0956-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a0956-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0956-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0956-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0956-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0956-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0956-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0956-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0956-114">Application</span></span> | <span data-ttu-id="a0956-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0956-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0956-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0956-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="a0956-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0956-117">Optional request headers</span></span>

| <span data-ttu-id="a0956-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a0956-118">Name</span></span>          | <span data-ttu-id="a0956-119">Тип</span><span class="sxs-lookup"><span data-stu-id="a0956-119">Type</span></span>   | <span data-ttu-id="a0956-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a0956-120">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a0956-121">if-match</span><span class="sxs-lookup"><span data-stu-id="a0956-121">if-match</span></span>      | <span data-ttu-id="a0956-122">String</span><span class="sxs-lookup"><span data-stu-id="a0956-122">String</span></span> | <span data-ttu-id="a0956-123">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом eTag папки, то возвращается отклик `412 Precondition Failed`.</span><span class="sxs-lookup"><span data-stu-id="a0956-123">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0956-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a0956-124">Request body</span></span>

<span data-ttu-id="a0956-125">Укажите в тексте запроса значения обновляемых свойств.</span><span class="sxs-lookup"><span data-stu-id="a0956-125">In the request body, supply the values for properties that should be updated.</span></span>

<span data-ttu-id="a0956-126">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="a0956-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="a0956-127">Для достижения максимальной оптимальной производительности в приложении не следует указывать свойства, которые не были изменены.</span><span class="sxs-lookup"><span data-stu-id="a0956-127">For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="a0956-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0956-128">Response</span></span>

<span data-ttu-id="a0956-129">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a0956-129">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0956-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a0956-130">Example</span></span>

<span data-ttu-id="a0956-131">В этом примере показано, как переименовать ресурс DriveItem и присвоить ему имя new-file-name.docx.</span><span class="sxs-lookup"><span data-stu-id="a0956-131">This example renames the DriveItem resource to "new-file-name.docx".</span></span>

<!-- { "blockType": "request", "name": "update-item" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```

### <a name="response"></a><span data-ttu-id="a0956-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="a0956-132">Response</span></span>

<span data-ttu-id="a0956-133">При успешном выполнении этот метод возвращает ресурс [driveItem][item-resource] в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a0956-133">If successful, this method returns an [driveItem][item-resource] resource in the response body.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a0956-134">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="a0956-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a0956-135">C#</span><span class="sxs-lookup"><span data-stu-id="a0956-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a0956-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0956-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update-item-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a0956-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a0956-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update-item-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="error-responses"></a><span data-ttu-id="a0956-138">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="a0956-138">Error responses</span></span>

<span data-ttu-id="a0956-139">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="a0956-139">See [Error Responses][error-response] for details about how errors are returned.</span></span>

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
    "Error: /api-reference/beta/api/driveitem-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitem-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
