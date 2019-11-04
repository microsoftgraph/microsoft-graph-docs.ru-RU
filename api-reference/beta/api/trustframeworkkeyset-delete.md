---
title: Удаление Трустфрамеворккэйсет
description: Удаление объекта **трустфрамеворккэйсет** .
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7ea8fcebe75e39397d62affc586a5db24cee7853
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938291"
---
# <a name="delete-trustframeworkkeyset"></a><span data-ttu-id="76482-103">Удаление Трустфрамеворккэйсет</span><span class="sxs-lookup"><span data-stu-id="76482-103">Delete trustFrameworkKeySet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76482-104">Удаление объекта [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="76482-104">Delete a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="76482-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76482-105">Permissions</span></span>

<span data-ttu-id="76482-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76482-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76482-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76482-108">Permission type</span></span>                        | <span data-ttu-id="76482-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76482-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="76482-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76482-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="76482-111">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="76482-111">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="76482-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76482-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76482-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76482-113">Not supported.</span></span> |
| <span data-ttu-id="76482-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76482-114">Application</span></span>                            | <span data-ttu-id="76482-115">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="76482-115">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76482-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76482-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="76482-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76482-117">Request headers</span></span>

| <span data-ttu-id="76482-118">Имя</span><span class="sxs-lookup"><span data-stu-id="76482-118">Name</span></span>          | <span data-ttu-id="76482-119">Описание</span><span class="sxs-lookup"><span data-stu-id="76482-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="76482-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76482-120">Authorization</span></span> | <span data-ttu-id="76482-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76482-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76482-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76482-123">Request body</span></span>

<span data-ttu-id="76482-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="76482-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76482-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="76482-125">Response</span></span>

<span data-ttu-id="76482-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="76482-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="76482-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="76482-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="76482-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="76482-129">Request</span></span>

<span data-ttu-id="76482-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76482-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="76482-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="76482-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_trustframeworkkeyset"
}-->

```http
DELETE https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="76482-132">C#</span><span class="sxs-lookup"><span data-stu-id="76482-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-trustframeworkkeyset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="76482-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76482-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-trustframeworkkeyset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="76482-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76482-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-trustframeworkkeyset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="76482-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="76482-135">Response</span></span>

<span data-ttu-id="76482-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="76482-136">The following is an example of the response.</span></span>

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
  "description": "Delete trustFrameworkKeySet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
