---
author: JeremyKelley
ms.author: jeremyke
title: Удаление элемента из пакета
description: Удаление элемента из набора элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: ff7f292be35b59f17465e65517174746faddca1a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944812"
---
# <a name="remove-item-from-bundle"></a><span data-ttu-id="1c63f-103">Удаление элемента из пакета</span><span class="sxs-lookup"><span data-stu-id="1c63f-103">Remove item from bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c63f-104">Удаление элемента из [пакета][].</span><span class="sxs-lookup"><span data-stu-id="1c63f-104">Remove an item from a [bundle][].</span></span>

## <a name="permissions"></a><span data-ttu-id="1c63f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c63f-105">Permissions</span></span>

<span data-ttu-id="1c63f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c63f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c63f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c63f-108">Permission type</span></span>      | <span data-ttu-id="1c63f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c63f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c63f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c63f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1c63f-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c63f-111">Not supported.</span></span>                             |
|<span data-ttu-id="1c63f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c63f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c63f-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c63f-113">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="1c63f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c63f-114">Application</span></span>          | <span data-ttu-id="1c63f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c63f-115">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="1c63f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c63f-116">HTTP request</span></span>

```http
DELETE /drive/bundles/{bundle-id}/children/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="1c63f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c63f-117">Request headers</span></span>

| <span data-ttu-id="1c63f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1c63f-118">Name</span></span>          | <span data-ttu-id="1c63f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1c63f-119">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="1c63f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c63f-120">Authorization</span></span> | <span data-ttu-id="1c63f-121">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="1c63f-121">Bearer \{token\}.</span></span> <span data-ttu-id="1c63f-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="1c63f-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c63f-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1c63f-123">Request body</span></span>

<span data-ttu-id="1c63f-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c63f-124">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c63f-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c63f-125">Response</span></span>

<span data-ttu-id="1c63f-126">В случае успеха отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1c63f-126">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="1c63f-127">Ознакомьтесь с разделом [ответы об ошибках][error-response] для получения дополнительных сведений об возвращении ошибок.</span><span class="sxs-lookup"><span data-stu-id="1c63f-127">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="1c63f-128">Пример</span><span class="sxs-lookup"><span data-stu-id="1c63f-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c63f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c63f-129">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1c63f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c63f-130">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "remove-from-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1c63f-131">C#</span><span class="sxs-lookup"><span data-stu-id="1c63f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-from-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1c63f-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="1c63f-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-from-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1c63f-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1c63f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-from-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1c63f-134">Java</span><span class="sxs-lookup"><span data-stu-id="1c63f-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-from-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1c63f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c63f-135">Response</span></span>

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
