---
author: JeremyKelley
ms.author: jeremyke
title: Удаление элемента из пакета
description: Удаление элемента из набора элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 508dd19edcd3c1ae231c54cdb195d86661bb4259
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441027"
---
# <a name="remove-item-from-bundle"></a><span data-ttu-id="a0545-103">Удаление элемента из пакета</span><span class="sxs-lookup"><span data-stu-id="a0545-103">Remove item from bundle</span></span>

<span data-ttu-id="a0545-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a0545-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0545-105">Удаление элемента из [пакета][].</span><span class="sxs-lookup"><span data-stu-id="a0545-105">Remove an item from a [bundle][].</span></span>

## <a name="permissions"></a><span data-ttu-id="a0545-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a0545-106">Permissions</span></span>

<span data-ttu-id="a0545-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0545-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0545-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a0545-109">Permission type</span></span>      | <span data-ttu-id="a0545-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a0545-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0545-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a0545-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a0545-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0545-112">Not supported.</span></span>                             |
|<span data-ttu-id="a0545-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a0545-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0545-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0545-114">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="a0545-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a0545-115">Application</span></span>          | <span data-ttu-id="a0545-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0545-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="a0545-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a0545-117">HTTP request</span></span>

```http
DELETE /drive/bundles/{bundle-id}/children/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="a0545-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a0545-118">Request headers</span></span>

| <span data-ttu-id="a0545-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a0545-119">Name</span></span>          | <span data-ttu-id="a0545-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a0545-120">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="a0545-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0545-121">Authorization</span></span> | <span data-ttu-id="a0545-122">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="a0545-122">Bearer \{token\}.</span></span> <span data-ttu-id="a0545-123">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="a0545-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0545-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a0545-124">Request body</span></span>

<span data-ttu-id="a0545-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a0545-125">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0545-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0545-126">Response</span></span>

<span data-ttu-id="a0545-127">В случае успеха отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a0545-127">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="a0545-128">Ознакомьтесь с разделом [ответы об ошибках][error-response] для получения дополнительных сведений об возвращении ошибок.</span><span class="sxs-lookup"><span data-stu-id="a0545-128">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="a0545-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a0545-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0545-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a0545-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a0545-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0545-131">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "remove-from-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children/{item-id}
```
# <a name="c"></a>[<span data-ttu-id="a0545-132">C#</span><span class="sxs-lookup"><span data-stu-id="a0545-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-from-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0545-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0545-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-from-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0545-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0545-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-from-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a0545-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a0545-135">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


[bundle]: ../resources/bundle.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Remove an item from a bundle.",
  "keywords": "",
  "section": "documentation"
} -->
