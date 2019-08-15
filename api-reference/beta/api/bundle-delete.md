---
author: JeremyKelley
ms.author: jeremyke
title: Удаление пакета
description: Удаление пакета элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 7556edc226f655af748facea1df6ea19820b7c9e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419263"
---
# <a name="delete-bundle"></a><span data-ttu-id="68db3-103">Удаление пакета</span><span class="sxs-lookup"><span data-stu-id="68db3-103">Delete bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68db3-104">Удаление [пакета][] элементов driveitem с помощью **идентификатора**. Обратите внимание, что удаление пакета с помощью этого метода окончательно удаляет пакет и не перемещает его в корзину.</span><span class="sxs-lookup"><span data-stu-id="68db3-104">Delete a [bundle][] of driveItems by using its **id**. Note that deleting a bundle using this method permanently deletes the bundle and does not move it to the Recycle Bin.</span></span>
<span data-ttu-id="68db3-105">Тем не менее, они не удаляют элементы, на которые ссылается пакет.</span><span class="sxs-lookup"><span data-stu-id="68db3-105">It does not, however, remove the items that were referenced by the bundle.</span></span>
<span data-ttu-id="68db3-106">Они останутся в своих родительских папках.</span><span class="sxs-lookup"><span data-stu-id="68db3-106">They will remain in their parent folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="68db3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68db3-107">Permissions</span></span>

<span data-ttu-id="68db3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68db3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68db3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68db3-110">Permission type</span></span>      | <span data-ttu-id="68db3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68db3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68db3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68db3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="68db3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68db3-113">Not supported.</span></span>                             |
|<span data-ttu-id="68db3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68db3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68db3-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68db3-115">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="68db3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68db3-116">Application</span></span>          | <span data-ttu-id="68db3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68db3-117">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="68db3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68db3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="68db3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68db3-119">Request headers</span></span>

| <span data-ttu-id="68db3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="68db3-120">Name</span></span>          | <span data-ttu-id="68db3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="68db3-121">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="68db3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68db3-122">Authorization</span></span> | <span data-ttu-id="68db3-123">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="68db3-123">Bearer \{token\}.</span></span> <span data-ttu-id="68db3-124">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68db3-124">Required.</span></span> |
| <span data-ttu-id="68db3-125">if-match</span><span class="sxs-lookup"><span data-stu-id="68db3-125">if-match</span></span>      | <span data-ttu-id="68db3-126">тегом.</span><span class="sxs-lookup"><span data-stu-id="68db3-126">eTag.</span></span> <span data-ttu-id="68db3-127">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="68db3-127">Optional.</span></span> <span data-ttu-id="68db3-128">Если указан заголовок запроса, а предоставленное значение eTag (или cTag) не совпадают с текущим тегом в пакете, возвращается `412 Precondition Failed` ответ и пакет не удаляется.</span><span class="sxs-lookup"><span data-stu-id="68db3-128">If this request header is included and the eTag (or cTag) provided does not match the current tag on the bundle, a `412 Precondition Failed` response is returned and the bundle will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="68db3-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="68db3-129">Request body</span></span>

<span data-ttu-id="68db3-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68db3-130">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="68db3-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="68db3-131">Response</span></span>

<span data-ttu-id="68db3-132">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="68db3-132">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<span data-ttu-id="68db3-133">Ознакомьтесь с разделом [ответы об ошибках][error-response] для получения дополнительных сведений об возвращении ошибок.</span><span class="sxs-lookup"><span data-stu-id="68db3-133">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="68db3-134">Пример</span><span class="sxs-lookup"><span data-stu-id="68db3-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="68db3-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="68db3-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="68db3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="68db3-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/items/{bundle-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="68db3-137">C#</span><span class="sxs-lookup"><span data-stu-id="68db3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68db3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68db3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="68db3-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="68db3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="68db3-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="68db3-140">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


[bundle]: ../resources/bundle.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a bundle from OneDrive",
  "keywords": "delete,existing bundle,onedrive",
  "section": "documentation",
  "tocPath": "Bundles/Delete"
} -->
