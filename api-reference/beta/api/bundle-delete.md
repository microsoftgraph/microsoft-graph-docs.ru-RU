---
author: JeremyKelley
ms.author: jeremyke
title: Удаление пакета
description: Удаление пакета элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 13cc2dcb3cda7dac8d6f9b7acfae153d84efabfa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987774"
---
# <a name="delete-bundle"></a><span data-ttu-id="54075-103">Удаление пакета</span><span class="sxs-lookup"><span data-stu-id="54075-103">Delete bundle</span></span>

<span data-ttu-id="54075-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54075-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54075-105">Удаление [пакета][] элементов driveitem с помощью **идентификатора**. Обратите внимание, что удаление пакета с помощью этого метода окончательно удаляет пакет и не перемещает его в корзину.</span><span class="sxs-lookup"><span data-stu-id="54075-105">Delete a [bundle][] of driveItems by using its **id**. Note that deleting a bundle using this method permanently deletes the bundle and does not move it to the Recycle Bin.</span></span>
<span data-ttu-id="54075-106">Тем не менее, они не удаляют элементы, на которые ссылается пакет.</span><span class="sxs-lookup"><span data-stu-id="54075-106">It does not, however, remove the items that were referenced by the bundle.</span></span>
<span data-ttu-id="54075-107">Они останутся в своих родительских папках.</span><span class="sxs-lookup"><span data-stu-id="54075-107">They will remain in their parent folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="54075-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54075-108">Permissions</span></span>

<span data-ttu-id="54075-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54075-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54075-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54075-111">Permission type</span></span>      | <span data-ttu-id="54075-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54075-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54075-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54075-113">Delegated (work or school account)</span></span> | <span data-ttu-id="54075-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54075-114">Not supported.</span></span>                             |
|<span data-ttu-id="54075-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54075-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54075-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54075-116">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="54075-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54075-117">Application</span></span>          | <span data-ttu-id="54075-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54075-118">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="54075-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54075-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="54075-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54075-120">Request headers</span></span>

| <span data-ttu-id="54075-121">Имя</span><span class="sxs-lookup"><span data-stu-id="54075-121">Name</span></span>          | <span data-ttu-id="54075-122">Описание</span><span class="sxs-lookup"><span data-stu-id="54075-122">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="54075-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="54075-123">Authorization</span></span> | <span data-ttu-id="54075-124">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="54075-124">Bearer \{token\}.</span></span> <span data-ttu-id="54075-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54075-125">Required.</span></span> |
| <span data-ttu-id="54075-126">if-match</span><span class="sxs-lookup"><span data-stu-id="54075-126">if-match</span></span>      | <span data-ttu-id="54075-127">тегом.</span><span class="sxs-lookup"><span data-stu-id="54075-127">eTag.</span></span> <span data-ttu-id="54075-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="54075-128">Optional.</span></span> <span data-ttu-id="54075-129">Если указан заголовок запроса, а предоставленное значение eTag (или cTag) не совпадают с текущим тегом в пакете, `412 Precondition Failed` возвращается ответ и пакет не удаляется.</span><span class="sxs-lookup"><span data-stu-id="54075-129">If this request header is included and the eTag (or cTag) provided does not match the current tag on the bundle, a `412 Precondition Failed` response is returned and the bundle will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="54075-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="54075-130">Request body</span></span>

<span data-ttu-id="54075-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54075-131">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="54075-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="54075-132">Response</span></span>

<span data-ttu-id="54075-133">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="54075-133">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<span data-ttu-id="54075-134">Ознакомьтесь с разделом [ответы об ошибках][error-response] для получения дополнительных сведений об возвращении ошибок.</span><span class="sxs-lookup"><span data-stu-id="54075-134">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="54075-135">Пример</span><span class="sxs-lookup"><span data-stu-id="54075-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="54075-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="54075-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="54075-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="54075-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/items/{bundle-id}
```
# <a name="c"></a>[<span data-ttu-id="54075-138">C#</span><span class="sxs-lookup"><span data-stu-id="54075-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54075-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54075-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54075-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54075-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="54075-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="54075-141">Response</span></span>

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


