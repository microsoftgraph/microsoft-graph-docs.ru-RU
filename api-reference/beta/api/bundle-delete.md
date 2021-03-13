---
author: JeremyKelley
title: Удаление пакета
description: Удаление пакета driveItems
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 737a5f7494ea0848e4776058e8f55b78df44e29a
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50774273"
---
# <a name="delete-bundle"></a><span data-ttu-id="2b303-103">Удаление пакета</span><span class="sxs-lookup"><span data-stu-id="2b303-103">Delete bundle</span></span>

<span data-ttu-id="2b303-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b303-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b303-105">Удаление [пакета][] driveItems с помощью **его id.** Обратите внимание, что удаление пакета с помощью этого метода навсегда удаляет пакет и не перемещает его в корзину.</span><span class="sxs-lookup"><span data-stu-id="2b303-105">Delete a [bundle][] of driveItems by using its **id**. Note that deleting a bundle using this method permanently deletes the bundle and does not move it to the Recycle Bin.</span></span>
<span data-ttu-id="2b303-106">Однако он не удаляет элементы, на которые ссылается пакет.</span><span class="sxs-lookup"><span data-stu-id="2b303-106">It does not, however, remove the items that were referenced by the bundle.</span></span>
<span data-ttu-id="2b303-107">Они останутся в родительских папках.</span><span class="sxs-lookup"><span data-stu-id="2b303-107">They will remain in their parent folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b303-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b303-108">Permissions</span></span>

<span data-ttu-id="2b303-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b303-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b303-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b303-111">Permission type</span></span>      | <span data-ttu-id="2b303-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b303-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b303-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b303-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2b303-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b303-114">Not supported.</span></span>                             |
|<span data-ttu-id="2b303-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b303-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b303-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b303-116">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="2b303-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b303-117">Application</span></span>          | <span data-ttu-id="2b303-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b303-118">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="2b303-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b303-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="2b303-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b303-120">Request headers</span></span>

| <span data-ttu-id="2b303-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2b303-121">Name</span></span>          | <span data-ttu-id="2b303-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2b303-122">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="2b303-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b303-123">Authorization</span></span> | <span data-ttu-id="2b303-124">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="2b303-124">Bearer \{token\}.</span></span> <span data-ttu-id="2b303-125">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b303-125">Required.</span></span> |
| <span data-ttu-id="2b303-126">if-match</span><span class="sxs-lookup"><span data-stu-id="2b303-126">if-match</span></span>      | <span data-ttu-id="2b303-127">eTag.</span><span class="sxs-lookup"><span data-stu-id="2b303-127">eTag.</span></span> <span data-ttu-id="2b303-128">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="2b303-128">Optional.</span></span> <span data-ttu-id="2b303-129">Если этот загон запроса включен, а предоставленный eTag (или cTag) не соответствует текущему тегу в пакете, возвращается ответ и пакет не `412 Precondition Failed` удаляется.</span><span class="sxs-lookup"><span data-stu-id="2b303-129">If this request header is included and the eTag (or cTag) provided does not match the current tag on the bundle, a `412 Precondition Failed` response is returned and the bundle will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="2b303-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2b303-130">Request body</span></span>

<span data-ttu-id="2b303-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b303-131">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b303-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b303-132">Response</span></span>

<span data-ttu-id="2b303-133">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="2b303-133">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<span data-ttu-id="2b303-134">Дополнительные сведения о возвращении ошибок см. в статье [Отклики с ошибками][error-response].</span><span class="sxs-lookup"><span data-stu-id="2b303-134">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="2b303-135">Пример</span><span class="sxs-lookup"><span data-stu-id="2b303-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b303-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b303-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2b303-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b303-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/items/{bundle-id}
```
# <a name="c"></a>[<span data-ttu-id="2b303-138">C#</span><span class="sxs-lookup"><span data-stu-id="2b303-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b303-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b303-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b303-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b303-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b303-141">Java</span><span class="sxs-lookup"><span data-stu-id="2b303-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2b303-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b303-142">Response</span></span>

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


