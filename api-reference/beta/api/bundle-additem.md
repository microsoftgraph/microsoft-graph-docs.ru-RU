---
author: JeremyKelley
ms.author: jeremyke
title: Добавление элемента в пакет
description: Добавление элемента в пакет элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: f6680d4903111301f61f11f1975596386dd263be
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944844"
---
# <a name="add-item-to-a-bundle"></a><span data-ttu-id="2415a-103">Добавление элемента в пакет</span><span class="sxs-lookup"><span data-stu-id="2415a-103">Add item to a bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2415a-104">Добавление дополнительного [driveItem][] с диска в [пакет][].</span><span class="sxs-lookup"><span data-stu-id="2415a-104">Add an additional [driveItem][] from a drive to a [bundle][].</span></span>

[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a><span data-ttu-id="2415a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2415a-107">Permissions</span></span>

<span data-ttu-id="2415a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2415a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2415a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2415a-110">Permission type</span></span>      | <span data-ttu-id="2415a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2415a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2415a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2415a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2415a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2415a-113">Not supported.</span></span>                             |
|<span data-ttu-id="2415a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2415a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2415a-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2415a-115">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="2415a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2415a-116">Application</span></span>          | <span data-ttu-id="2415a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2415a-117">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="2415a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2415a-118">HTTP request</span></span>

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a><span data-ttu-id="2415a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2415a-119">Request headers</span></span>

| <span data-ttu-id="2415a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2415a-120">Name</span></span>          | <span data-ttu-id="2415a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2415a-121">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="2415a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2415a-122">Authorization</span></span> | <span data-ttu-id="2415a-123">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="2415a-123">Bearer \{token\}.</span></span> <span data-ttu-id="2415a-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="2415a-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2415a-125">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="2415a-125">Request body</span></span>

<span data-ttu-id="2415a-126">Текст запроса включает идентификатор для элемента, который следует добавить в коллекцию Children набора.</span><span class="sxs-lookup"><span data-stu-id="2415a-126">The request body includes the identifier for an item that should be added to the bundle's children collection.</span></span>

## <a name="response"></a><span data-ttu-id="2415a-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2415a-127">Response</span></span>

<span data-ttu-id="2415a-128">В случае успеха отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2415a-128">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="2415a-129">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="2415a-129">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="2415a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2415a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2415a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2415a-131">Request</span></span>

<span data-ttu-id="2415a-132">Этот запрос добавит существующий элемент в указанный пакет.</span><span class="sxs-lookup"><span data-stu-id="2415a-132">This request will add an existing item to the specified bundle.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2415a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2415a-133">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2415a-134">C#</span><span class="sxs-lookup"><span data-stu-id="2415a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-to-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2415a-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="2415a-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-to-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2415a-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2415a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-to-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2415a-137">Java</span><span class="sxs-lookup"><span data-stu-id="2415a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-to-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2415a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2415a-138">Response</span></span>

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
