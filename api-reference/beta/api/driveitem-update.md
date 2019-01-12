---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Обновление файла или папки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e634cbba53a3eeca2f86f8bbfb63beb4ac0baa08
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985531"
---
# <a name="update-driveitem-properties"></a><span data-ttu-id="0c3c0-102">Обновление свойств ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="0c3c0-102">Update DriveItem properties</span></span>

> <span data-ttu-id="0c3c0-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c3c0-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c3c0-105">Обновление метаданных ресурса [DriveItem](../resources/driveitem.md) по идентификатору или пути.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-105">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="0c3c0-106">Путем обновления также можно [переместить элемент](driveitem-move.md) в другой родительский объект, изменив свойство **parentReference** этого элемента.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-106">You can also use update to [move an item](driveitem-move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c3c0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c3c0-107">Permissions</span></span>

<span data-ttu-id="0c3c0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c3c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c3c0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c3c0-110">Permission type</span></span>      | <span data-ttu-id="0c3c0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c3c0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c3c0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c3c0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0c3c0-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c3c0-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0c3c0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c3c0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c3c0-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c3c0-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0c3c0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c3c0-116">Application</span></span> | <span data-ttu-id="0c3c0-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c3c0-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c3c0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c3c0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="0c3c0-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c3c0-119">Optional request headers</span></span>

| <span data-ttu-id="0c3c0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0c3c0-120">Name</span></span>          | <span data-ttu-id="0c3c0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0c3c0-121">Type</span></span>   | <span data-ttu-id="0c3c0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0c3c0-122">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0c3c0-123">if-match</span><span class="sxs-lookup"><span data-stu-id="0c3c0-123">if-match</span></span>      | <span data-ttu-id="0c3c0-124">String</span><span class="sxs-lookup"><span data-stu-id="0c3c0-124">String</span></span> | <span data-ttu-id="0c3c0-125">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом eTag папки, то возвращается отклик `412 Precondition Failed`.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-125">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0c3c0-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0c3c0-126">Request body</span></span>

<span data-ttu-id="0c3c0-127">Укажите в тексте запроса значения обновляемых свойств.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-127">In the request body, supply the values for properties that should be updated.</span></span>

<span data-ttu-id="0c3c0-128">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="0c3c0-129">Для достижения максимальной оптимальной производительности в приложении не следует указывать свойства, которые не были изменены.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-129">For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="0c3c0-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c3c0-130">Response</span></span>

<span data-ttu-id="0c3c0-131">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный ресурс [DriveItem](../resources/driveitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-131">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c3c0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0c3c0-132">Example</span></span>

<span data-ttu-id="0c3c0-133">В этом примере показано, как переименовать ресурс DriveItem и присвоить ему имя new-file-name.docx.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-133">This example renames the DriveItem resource to "new-file-name.docx".</span></span>

<!-- { "blockType": "request", "name": "update-item" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```

### <a name="response"></a><span data-ttu-id="0c3c0-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c3c0-134">Response</span></span>

<span data-ttu-id="0c3c0-135">При успешном выполнении этот метод возвращает ресурс [driveItem][item-resource] в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0c3c0-135">If successful, this method returns an [driveItem][item-resource] resource in the response body.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="0c3c0-136">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="0c3c0-136">Error responses</span></span>

<span data-ttu-id="0c3c0-137">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="0c3c0-137">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of an item.",
  "keywords": "update,replace,contents,item",
  "section": "documentation",
  "tocPath": "Items/Update"
} -->
