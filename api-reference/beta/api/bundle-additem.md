---
author: JeremyKelley
ms.author: jeremyke
title: Добавление элемента в пакет
description: Добавление элемента в пакет элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c192014a00e3a2119691857c8350dc03d53e1980
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441055"
---
# <a name="add-item-to-a-bundle"></a><span data-ttu-id="7fc68-103">Добавление элемента в пакет</span><span class="sxs-lookup"><span data-stu-id="7fc68-103">Add item to a bundle</span></span>

<span data-ttu-id="7fc68-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7fc68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fc68-105">Добавление дополнительного [driveItem][] с диска в [пакет][].</span><span class="sxs-lookup"><span data-stu-id="7fc68-105">Add an additional [driveItem][] from a drive to a [bundle][].</span></span>

[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a><span data-ttu-id="7fc68-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7fc68-108">Permissions</span></span>

<span data-ttu-id="7fc68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fc68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fc68-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fc68-111">Permission type</span></span>      | <span data-ttu-id="7fc68-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fc68-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fc68-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fc68-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7fc68-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fc68-114">Not supported.</span></span>                             |
|<span data-ttu-id="7fc68-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fc68-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fc68-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fc68-116">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="7fc68-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fc68-117">Application</span></span>          | <span data-ttu-id="7fc68-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fc68-118">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="7fc68-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fc68-119">HTTP request</span></span>

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a><span data-ttu-id="7fc68-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7fc68-120">Request headers</span></span>

| <span data-ttu-id="7fc68-121">Имя</span><span class="sxs-lookup"><span data-stu-id="7fc68-121">Name</span></span>          | <span data-ttu-id="7fc68-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7fc68-122">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="7fc68-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7fc68-123">Authorization</span></span> | <span data-ttu-id="7fc68-124">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="7fc68-124">Bearer \{token\}.</span></span> <span data-ttu-id="7fc68-125">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="7fc68-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7fc68-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7fc68-126">Request body</span></span>

<span data-ttu-id="7fc68-127">Текст запроса включает идентификатор для элемента, который следует добавить в коллекцию Children набора.</span><span class="sxs-lookup"><span data-stu-id="7fc68-127">The request body includes the identifier for an item that should be added to the bundle's children collection.</span></span>

## <a name="response"></a><span data-ttu-id="7fc68-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fc68-128">Response</span></span>

<span data-ttu-id="7fc68-129">В случае успеха отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7fc68-129">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="7fc68-130">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="7fc68-130">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="7fc68-131">Пример</span><span class="sxs-lookup"><span data-stu-id="7fc68-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fc68-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fc68-132">Request</span></span>

<span data-ttu-id="7fc68-133">Этот запрос добавит существующий элемент в указанный пакет.</span><span class="sxs-lookup"><span data-stu-id="7fc68-133">This request will add an existing item to the specified bundle.</span></span>


# <a name="http"></a>[<span data-ttu-id="7fc68-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fc68-134">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```
# <a name="c"></a>[<span data-ttu-id="7fc68-135">C#</span><span class="sxs-lookup"><span data-stu-id="7fc68-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-to-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fc68-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fc68-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-to-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fc68-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fc68-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-to-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7fc68-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fc68-138">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Add items to an existing bundle.",
  "keywords": "",
  "section": "documentation"
} -->
