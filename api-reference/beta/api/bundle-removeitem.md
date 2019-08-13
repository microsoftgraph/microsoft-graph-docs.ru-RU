---
author: JeremyKelley
ms.author: jeremyke
title: Удаление элемента из пакета
description: Удаление элемента из набора элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: a6229b56700b11d7c56599bb23e4799e1d7021a6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317982"
---
# <a name="remove-item-from-bundle"></a><span data-ttu-id="618cb-103">Удаление элемента из пакета</span><span class="sxs-lookup"><span data-stu-id="618cb-103">Remove item from bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="618cb-104">Удаление элемента из [пакета][].</span><span class="sxs-lookup"><span data-stu-id="618cb-104">Remove an item from a [bundle][].</span></span>

## <a name="permissions"></a><span data-ttu-id="618cb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="618cb-105">Permissions</span></span>

<span data-ttu-id="618cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="618cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="618cb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="618cb-108">Permission type</span></span>      | <span data-ttu-id="618cb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="618cb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="618cb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="618cb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="618cb-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="618cb-111">Not supported.</span></span>                             |
|<span data-ttu-id="618cb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="618cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="618cb-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="618cb-113">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="618cb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="618cb-114">Application</span></span>          | <span data-ttu-id="618cb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="618cb-115">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="618cb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="618cb-116">HTTP request</span></span>

```http
DELETE /drive/bundles/{bundle-id}/children/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="618cb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="618cb-117">Request headers</span></span>

| <span data-ttu-id="618cb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="618cb-118">Name</span></span>          | <span data-ttu-id="618cb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="618cb-119">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="618cb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="618cb-120">Authorization</span></span> | <span data-ttu-id="618cb-121">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="618cb-121">Bearer \{token\}.</span></span> <span data-ttu-id="618cb-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="618cb-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="618cb-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="618cb-123">Request body</span></span>

<span data-ttu-id="618cb-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="618cb-124">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="618cb-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="618cb-125">Response</span></span>

<span data-ttu-id="618cb-126">В случае успеха отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="618cb-126">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="618cb-127">Ознакомьтесь с разделом [ответы об ошибках][error-response] для получения дополнительных сведений об возвращении ошибок.</span><span class="sxs-lookup"><span data-stu-id="618cb-127">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="618cb-128">Пример</span><span class="sxs-lookup"><span data-stu-id="618cb-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="618cb-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="618cb-129">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="618cb-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="618cb-130">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "remove-from-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="618cb-131">C#</span><span class="sxs-lookup"><span data-stu-id="618cb-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-from-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="618cb-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="618cb-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-from-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="618cb-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="618cb-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-from-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="618cb-134">Java</span><span class="sxs-lookup"><span data-stu-id="618cb-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-from-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="618cb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="618cb-135">Response</span></span>

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
