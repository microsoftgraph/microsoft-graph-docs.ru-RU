---
title: Удаление Акцесспаккажекаталог
description: Удаление Акцесспаккажекаталог.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 063b2baff5ad2bae4ff9ea68e32daf689ceca6dc
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994340"
---
# <a name="delete-accesspackagecatalog"></a><span data-ttu-id="842ee-103">Удаление Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="842ee-103">Delete accessPackageCatalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="842ee-104">Удаление [акцесспаккажекаталог](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="842ee-104">Delete an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="842ee-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="842ee-105">Permissions</span></span>

<span data-ttu-id="842ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="842ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="842ee-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="842ee-108">Permission type</span></span>                        | <span data-ttu-id="842ee-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="842ee-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="842ee-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="842ee-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="842ee-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="842ee-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="842ee-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="842ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="842ee-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="842ee-113">Not supported.</span></span> |
| <span data-ttu-id="842ee-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="842ee-114">Application</span></span>                            | <span data-ttu-id="842ee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="842ee-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="842ee-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="842ee-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="842ee-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="842ee-117">Request headers</span></span>

| <span data-ttu-id="842ee-118">Имя</span><span class="sxs-lookup"><span data-stu-id="842ee-118">Name</span></span>          | <span data-ttu-id="842ee-119">Описание</span><span class="sxs-lookup"><span data-stu-id="842ee-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="842ee-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="842ee-120">Authorization</span></span> | <span data-ttu-id="842ee-121">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="842ee-121">Bearer \{token\}.</span></span> <span data-ttu-id="842ee-122">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="842ee-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="842ee-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="842ee-123">Request body</span></span>

<span data-ttu-id="842ee-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="842ee-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="842ee-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="842ee-125">Response</span></span>

<span data-ttu-id="842ee-126">В случае успешного выполнения этот метод возвращает код ответа серии 200.</span><span class="sxs-lookup"><span data-stu-id="842ee-126">If successful, this method returns a 200-series response code.</span></span> <span data-ttu-id="842ee-127">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="842ee-127">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="842ee-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="842ee-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="842ee-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="842ee-129">Request</span></span>

<span data-ttu-id="842ee-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="842ee-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="842ee-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="842ee-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accesspackagecatalog"
}-->

```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="842ee-132">C#</span><span class="sxs-lookup"><span data-stu-id="842ee-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="842ee-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="842ee-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="842ee-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="842ee-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="842ee-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="842ee-135">Response</span></span>

<span data-ttu-id="842ee-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="842ee-136">The following is an example of the response.</span></span>

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
  "description": "Delete accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
