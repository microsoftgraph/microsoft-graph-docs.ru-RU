---
author: JeremyKelley
ms.author: jeremyke
title: Добавление элемента в пакет
description: Добавление элемента в пакет элементов driveitem
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: a5b764bf94894d77ccead6adaa205882f6723fc5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960306"
---
# <a name="add-item-to-a-bundle"></a><span data-ttu-id="326bd-103">Добавление элемента в пакет</span><span class="sxs-lookup"><span data-stu-id="326bd-103">Add item to a bundle</span></span>

<span data-ttu-id="326bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="326bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="326bd-105">Добавление дополнительного [driveItem][] с диска в [пакет][].</span><span class="sxs-lookup"><span data-stu-id="326bd-105">Add an additional [driveItem][] from a drive to a [bundle][].</span></span>

[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a><span data-ttu-id="326bd-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="326bd-108">Permissions</span></span>

<span data-ttu-id="326bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="326bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="326bd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="326bd-111">Permission type</span></span>      | <span data-ttu-id="326bd-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="326bd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="326bd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="326bd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="326bd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="326bd-114">Not supported.</span></span>                             |
|<span data-ttu-id="326bd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="326bd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="326bd-116">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="326bd-116">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="326bd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="326bd-117">Application</span></span>          | <span data-ttu-id="326bd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="326bd-118">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="326bd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="326bd-119">HTTP request</span></span>

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a><span data-ttu-id="326bd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="326bd-120">Request headers</span></span>

| <span data-ttu-id="326bd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="326bd-121">Name</span></span>          | <span data-ttu-id="326bd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="326bd-122">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="326bd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="326bd-123">Authorization</span></span> | <span data-ttu-id="326bd-124">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="326bd-124">Bearer \{token\}.</span></span> <span data-ttu-id="326bd-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="326bd-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="326bd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="326bd-126">Request body</span></span>

<span data-ttu-id="326bd-127">Текст запроса включает идентификатор для элемента, который следует добавить в коллекцию Children набора.</span><span class="sxs-lookup"><span data-stu-id="326bd-127">The request body includes the identifier for an item that should be added to the bundle's children collection.</span></span>

## <a name="response"></a><span data-ttu-id="326bd-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="326bd-128">Response</span></span>

<span data-ttu-id="326bd-129">В случае успеха отклика `204 No Content` .</span><span class="sxs-lookup"><span data-stu-id="326bd-129">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="326bd-130">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="326bd-130">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="326bd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="326bd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="326bd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="326bd-132">Request</span></span>

<span data-ttu-id="326bd-133">Этот запрос добавит существующий элемент в указанный пакет.</span><span class="sxs-lookup"><span data-stu-id="326bd-133">This request will add an existing item to the specified bundle.</span></span>


# <a name="http"></a>[<span data-ttu-id="326bd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="326bd-134">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```
# <a name="c"></a>[<span data-ttu-id="326bd-135">C#</span><span class="sxs-lookup"><span data-stu-id="326bd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-to-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="326bd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="326bd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-to-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="326bd-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="326bd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-to-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="326bd-138">Java</span><span class="sxs-lookup"><span data-stu-id="326bd-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-to-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="326bd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="326bd-139">Response</span></span>

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


