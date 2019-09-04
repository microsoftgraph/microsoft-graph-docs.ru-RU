---
title: Удаление Цертификатебаседаусконфигуратион
description: Удаление Цертификатебаседаусконфигуратион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ce54ddecbaa166a64ba5379c09729af44baad7d8
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718759"
---
# <a name="delete-certificatebasedauthconfiguration"></a><span data-ttu-id="e70a6-103">Удаление Цертификатебаседаусконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e70a6-103">Delete certificateBasedAuthConfiguration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e70a6-104">Удаление объекта [цертификатебаседаусконфигуратион](../resources/certificateBasedAuthConfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e70a6-104">Delete a [certificateBasedAuthConfiguration](../resources/certificateBasedAuthConfiguration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e70a6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e70a6-105">Permissions</span></span>

<span data-ttu-id="e70a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e70a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e70a6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e70a6-108">Permission type</span></span>                        | <span data-ttu-id="e70a6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e70a6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e70a6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e70a6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e70a6-111">Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e70a6-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="e70a6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e70a6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e70a6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e70a6-113">Not supported.</span></span> |
| <span data-ttu-id="e70a6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e70a6-114">Application</span></span>    | <span data-ttu-id="e70a6-115">Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e70a6-115">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e70a6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e70a6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /organization/{id}/certificateBasedAuthConfiguration/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e70a6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e70a6-117">Request headers</span></span>

| <span data-ttu-id="e70a6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e70a6-118">Name</span></span>          | <span data-ttu-id="e70a6-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e70a6-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e70a6-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e70a6-120">Authorization</span></span> | <span data-ttu-id="e70a6-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="e70a6-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e70a6-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e70a6-122">Request body</span></span>

<span data-ttu-id="e70a6-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e70a6-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e70a6-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="e70a6-124">Response</span></span>

<span data-ttu-id="e70a6-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e70a6-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e70a6-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="e70a6-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e70a6-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="e70a6-128">Request</span></span>

<span data-ttu-id="e70a6-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e70a6-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e70a6-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e70a6-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_certificatebasedauthconfiguration"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/{id}/certificateBasedAuthConfiguration/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e70a6-131">C#</span><span class="sxs-lookup"><span data-stu-id="e70a6-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-certificatebasedauthconfiguration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e70a6-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e70a6-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-certificatebasedauthconfiguration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e70a6-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e70a6-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-certificatebasedauthconfiguration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e70a6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e70a6-134">Response</span></span>

<span data-ttu-id="e70a6-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e70a6-135">The following is an example of the response.</span></span>

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
  "description": "Delete certificateBasedAuthConfiguration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
