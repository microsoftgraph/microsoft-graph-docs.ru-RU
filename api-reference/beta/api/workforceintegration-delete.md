---
title: Удаление Воркфорцеинтегратион
description: Удаление экземпляра объекта Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 37ffb3e6153228963f8a0154f9f0c8708787ed98
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870540"
---
# <a name="delete-workforceintegration"></a><span data-ttu-id="2da51-103">Удаление Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="2da51-103">Delete workforceIntegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2da51-104">Удаление экземпляра объекта [воркфорцеинтегратион](../resources/workforceintegration.md).</span><span class="sxs-lookup"><span data-stu-id="2da51-104">Delete an instance of a [workforceIntegration](../resources/workforceintegration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2da51-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2da51-105">Permissions</span></span>

<span data-ttu-id="2da51-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2da51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2da51-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2da51-108">Permission type</span></span>                        | <span data-ttu-id="2da51-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2da51-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2da51-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2da51-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2da51-111">Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2da51-111">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="2da51-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2da51-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2da51-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2da51-113">Not supported.</span></span> |
| <span data-ttu-id="2da51-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2da51-114">Application</span></span>                            | <span data-ttu-id="2da51-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2da51-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2da51-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2da51-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="2da51-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2da51-117">Request headers</span></span>

| <span data-ttu-id="2da51-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2da51-118">Name</span></span>          | <span data-ttu-id="2da51-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2da51-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2da51-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2da51-120">Authorization</span></span> | <span data-ttu-id="2da51-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="2da51-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2da51-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2da51-122">Request body</span></span>

<span data-ttu-id="2da51-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2da51-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2da51-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="2da51-124">Response</span></span>

<span data-ttu-id="2da51-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2da51-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2da51-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="2da51-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2da51-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="2da51-128">Request</span></span>

<span data-ttu-id="2da51-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2da51-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2da51-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="2da51-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_workforceintegration"
}-->

```http
DELETE https://graph.microsoft.com/beta/teamwork/workforceIntegrations
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2da51-131">C#</span><span class="sxs-lookup"><span data-stu-id="2da51-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2da51-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2da51-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2da51-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2da51-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2da51-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2da51-134">Response</span></span>

<span data-ttu-id="2da51-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2da51-135">The following is an example of the response.</span></span>

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
  "description": "Delete workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
