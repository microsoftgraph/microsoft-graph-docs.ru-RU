---
title: Удаление индикатора службы угроз
description: Удаление объекта Тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 553bcecae386e03f10d19d43e443f666531b1684
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421276"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="35bfb-103">Удаление индикатора службы угроз</span><span class="sxs-lookup"><span data-stu-id="35bfb-103">Delete threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35bfb-104">Удаление объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="35bfb-104">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="35bfb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35bfb-105">Permissions</span></span>

<span data-ttu-id="35bfb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35bfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35bfb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35bfb-108">Permission type</span></span>                        | <span data-ttu-id="35bfb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35bfb-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="35bfb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35bfb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="35bfb-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="35bfb-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="35bfb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35bfb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35bfb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35bfb-113">Not supported.</span></span> |
| <span data-ttu-id="35bfb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35bfb-114">Application</span></span>                            | <span data-ttu-id="35bfb-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="35bfb-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="35bfb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35bfb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="35bfb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35bfb-117">Request headers</span></span>

| <span data-ttu-id="35bfb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="35bfb-118">Name</span></span>          | <span data-ttu-id="35bfb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="35bfb-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="35bfb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35bfb-120">Authorization</span></span> | <span data-ttu-id="35bfb-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="35bfb-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="35bfb-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35bfb-122">Request body</span></span>

<span data-ttu-id="35bfb-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35bfb-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35bfb-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="35bfb-124">Response</span></span>

<span data-ttu-id="35bfb-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="35bfb-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="35bfb-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="35bfb-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="35bfb-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="35bfb-128">Request</span></span>

<span data-ttu-id="35bfb-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35bfb-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="35bfb-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="35bfb-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="35bfb-131">C#</span><span class="sxs-lookup"><span data-stu-id="35bfb-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="35bfb-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35bfb-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="35bfb-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="35bfb-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="35bfb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="35bfb-134">Response</span></span>

<span data-ttu-id="35bfb-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="35bfb-135">The following is an example of the response.</span></span>

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
  "description": "Delete tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
