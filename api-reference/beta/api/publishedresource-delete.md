---
title: Удаление Публишедресаурце
description: Удаление объекта [публишедресаурце](../resources/publishedresource.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b617adce22e2671d75dc492cc278171f5e94a6c8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875214"
---
# <a name="delete-publishedresource"></a><span data-ttu-id="a8164-103">Удаление Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="a8164-103">Delete publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8164-104">Удаление объекта [публишедресаурце](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="a8164-104">Delete a [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8164-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8164-105">Permissions</span></span>

<span data-ttu-id="a8164-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8164-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8164-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8164-108">Permission type</span></span>                        | <span data-ttu-id="a8164-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8164-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="a8164-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8164-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8164-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a8164-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="a8164-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8164-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8164-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8164-113">Not supported.</span></span> |
| <span data-ttu-id="a8164-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8164-114">Application</span></span>                            | <span data-ttu-id="a8164-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8164-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8164-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8164-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="a8164-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8164-117">Request headers</span></span>

| <span data-ttu-id="a8164-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a8164-118">Name</span></span>          | <span data-ttu-id="a8164-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a8164-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a8164-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8164-120">Authorization</span></span> | <span data-ttu-id="a8164-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="a8164-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8164-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a8164-122">Request body</span></span>

<span data-ttu-id="a8164-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8164-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8164-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8164-124">Response</span></span>

<span data-ttu-id="a8164-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a8164-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a8164-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="a8164-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a8164-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8164-128">Request</span></span>

<span data-ttu-id="a8164-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8164-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a8164-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8164-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a8164-131">C#</span><span class="sxs-lookup"><span data-stu-id="a8164-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8164-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="a8164-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a8164-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a8164-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a8164-134">Java</span><span class="sxs-lookup"><span data-stu-id="a8164-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8164-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8164-135">Response</span></span>

<span data-ttu-id="a8164-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a8164-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
