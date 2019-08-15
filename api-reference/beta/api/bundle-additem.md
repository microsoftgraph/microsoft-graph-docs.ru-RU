---
author: JeremyKelley
ms.author: jeremyke
title: Добавление элемента в пакет
description: Добавление элемента в пакет элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e31fed6b88164ea305d820fb227ae71da9337226
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419250"
---
# <a name="add-item-to-a-bundle"></a><span data-ttu-id="74ab3-103">Добавление элемента в пакет</span><span class="sxs-lookup"><span data-stu-id="74ab3-103">Add item to a bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74ab3-104">Добавление дополнительного [driveItem][] с диска в [пакет][].</span><span class="sxs-lookup"><span data-stu-id="74ab3-104">Add an additional [driveItem][] from a drive to a [bundle][].</span></span>

[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a><span data-ttu-id="74ab3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="74ab3-107">Permissions</span></span>

<span data-ttu-id="74ab3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74ab3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74ab3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="74ab3-110">Permission type</span></span>      | <span data-ttu-id="74ab3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="74ab3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74ab3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="74ab3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="74ab3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74ab3-113">Not supported.</span></span>                             |
|<span data-ttu-id="74ab3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="74ab3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74ab3-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74ab3-115">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="74ab3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="74ab3-116">Application</span></span>          | <span data-ttu-id="74ab3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74ab3-117">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="74ab3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="74ab3-118">HTTP request</span></span>

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a><span data-ttu-id="74ab3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="74ab3-119">Request headers</span></span>

| <span data-ttu-id="74ab3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="74ab3-120">Name</span></span>          | <span data-ttu-id="74ab3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="74ab3-121">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="74ab3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="74ab3-122">Authorization</span></span> | <span data-ttu-id="74ab3-123">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="74ab3-123">Bearer \{token\}.</span></span> <span data-ttu-id="74ab3-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="74ab3-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74ab3-125">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="74ab3-125">Request body</span></span>

<span data-ttu-id="74ab3-126">Текст запроса включает идентификатор для элемента, который следует добавить в коллекцию Children набора.</span><span class="sxs-lookup"><span data-stu-id="74ab3-126">The request body includes the identifier for an item that should be added to the bundle's children collection.</span></span>

## <a name="response"></a><span data-ttu-id="74ab3-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="74ab3-127">Response</span></span>

<span data-ttu-id="74ab3-128">В случае успеха отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="74ab3-128">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="74ab3-129">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="74ab3-129">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="74ab3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="74ab3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="74ab3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="74ab3-131">Request</span></span>

<span data-ttu-id="74ab3-132">Этот запрос добавит существующий элемент в указанный пакет.</span><span class="sxs-lookup"><span data-stu-id="74ab3-132">This request will add an existing item to the specified bundle.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="74ab3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="74ab3-133">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="74ab3-134">C#</span><span class="sxs-lookup"><span data-stu-id="74ab3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-to-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74ab3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74ab3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-to-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="74ab3-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="74ab3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-to-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="74ab3-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="74ab3-137">Response</span></span>

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
