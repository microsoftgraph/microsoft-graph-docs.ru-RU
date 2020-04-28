---
title: Удаление Воркфорцеинтегратион
description: Удаление экземпляра объекта Воркфорцеинтегратион.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bb9d7a4259f4420971b9341e01acedd9da7049f2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451289"
---
# <a name="delete-workforceintegration"></a><span data-ttu-id="e9891-103">Удаление Воркфорцеинтегратион</span><span class="sxs-lookup"><span data-stu-id="e9891-103">Delete workforceIntegration</span></span>

<span data-ttu-id="e9891-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9891-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9891-105">Удаление экземпляра объекта [воркфорцеинтегратион](../resources/workforceintegration.md).</span><span class="sxs-lookup"><span data-stu-id="e9891-105">Delete an instance of a [workforceIntegration](../resources/workforceintegration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9891-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9891-106">Permissions</span></span>

<span data-ttu-id="e9891-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9891-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9891-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9891-109">Permission type</span></span>                        | <span data-ttu-id="e9891-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9891-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e9891-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9891-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9891-112">Воркфорцеинтегратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e9891-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="e9891-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9891-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9891-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9891-114">Not supported.</span></span> |
| <span data-ttu-id="e9891-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9891-115">Application</span></span>                            | <span data-ttu-id="e9891-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9891-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9891-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9891-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="e9891-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9891-118">Request headers</span></span>

| <span data-ttu-id="e9891-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e9891-119">Name</span></span>          | <span data-ttu-id="e9891-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e9891-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e9891-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9891-121">Authorization</span></span> | <span data-ttu-id="e9891-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="e9891-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9891-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9891-123">Request body</span></span>

<span data-ttu-id="e9891-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9891-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9891-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9891-125">Response</span></span>

<span data-ttu-id="e9891-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e9891-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9891-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="e9891-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e9891-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9891-129">Request</span></span>

<span data-ttu-id="e9891-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9891-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9891-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9891-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_workforceintegration"
}-->

```http
DELETE https://graph.microsoft.com/beta/teamwork/workforceIntegrations
```
# <a name="c"></a>[<span data-ttu-id="e9891-132">C#</span><span class="sxs-lookup"><span data-stu-id="e9891-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9891-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9891-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9891-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9891-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e9891-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9891-135">Response</span></span>

<span data-ttu-id="e9891-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e9891-136">The following is an example of the response.</span></span>

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
