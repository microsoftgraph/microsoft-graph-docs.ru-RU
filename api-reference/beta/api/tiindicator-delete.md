---
title: Удаление индикатора службы угроз
description: Удаление объекта Тииндикатор.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 790509aa9cc74dcd13ebcbed68e0e5816d6d0566
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362789"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="db42a-103">Удаление индикатора службы угроз</span><span class="sxs-lookup"><span data-stu-id="db42a-103">Delete threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db42a-104">Удаление объекта [тииндикатор](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="db42a-104">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="db42a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db42a-105">Permissions</span></span>

<span data-ttu-id="db42a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db42a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db42a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db42a-108">Permission type</span></span>                        | <span data-ttu-id="db42a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db42a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="db42a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db42a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="db42a-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="db42a-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="db42a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db42a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db42a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db42a-113">Not supported.</span></span> |
| <span data-ttu-id="db42a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db42a-114">Application</span></span>                            | <span data-ttu-id="db42a-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="db42a-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="db42a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db42a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="db42a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db42a-117">Request headers</span></span>

| <span data-ttu-id="db42a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="db42a-118">Name</span></span>          | <span data-ttu-id="db42a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="db42a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="db42a-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db42a-120">Authorization</span></span> | <span data-ttu-id="db42a-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="db42a-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="db42a-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db42a-122">Request body</span></span>

<span data-ttu-id="db42a-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db42a-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db42a-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="db42a-124">Response</span></span>

<span data-ttu-id="db42a-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="db42a-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db42a-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="db42a-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="db42a-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="db42a-128">Request</span></span>

<span data-ttu-id="db42a-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db42a-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db42a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="db42a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db42a-131">C#</span><span class="sxs-lookup"><span data-stu-id="db42a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db42a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db42a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db42a-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="db42a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="db42a-134">Java</span><span class="sxs-lookup"><span data-stu-id="db42a-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="db42a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="db42a-135">Response</span></span>

<span data-ttu-id="db42a-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="db42a-136">The following is an example of the response.</span></span>

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
