---
title: Удаление Трустфрамеворккэйсет
description: Удаление объекта **трустфрамеворккэйсет** .
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 309caf8eaa92f10ffdec9a1430a4a01fcd31d195
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981706"
---
# <a name="delete-trustframeworkkeyset"></a><span data-ttu-id="63b2b-103">Удаление Трустфрамеворккэйсет</span><span class="sxs-lookup"><span data-stu-id="63b2b-103">Delete trustFrameworkKeySet</span></span>

<span data-ttu-id="63b2b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63b2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63b2b-105">Удаление объекта [трустфрамеворккэйсет](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="63b2b-105">Delete a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="63b2b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63b2b-106">Permissions</span></span>

<span data-ttu-id="63b2b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63b2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63b2b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63b2b-109">Permission type</span></span>                        | <span data-ttu-id="63b2b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63b2b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="63b2b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63b2b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="63b2b-112">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="63b2b-112">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="63b2b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63b2b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63b2b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63b2b-114">Not supported.</span></span> |
| <span data-ttu-id="63b2b-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="63b2b-115">Application</span></span>                            | <span data-ttu-id="63b2b-116">Трустфрамеворккэйсет. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="63b2b-116">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="63b2b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63b2b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="63b2b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63b2b-118">Request headers</span></span>

| <span data-ttu-id="63b2b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="63b2b-119">Name</span></span>          | <span data-ttu-id="63b2b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="63b2b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="63b2b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63b2b-121">Authorization</span></span> | <span data-ttu-id="63b2b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63b2b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="63b2b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="63b2b-124">Request body</span></span>

<span data-ttu-id="63b2b-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63b2b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63b2b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="63b2b-126">Response</span></span>

<span data-ttu-id="63b2b-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="63b2b-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63b2b-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="63b2b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="63b2b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="63b2b-130">Request</span></span>

<span data-ttu-id="63b2b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63b2b-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63b2b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="63b2b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_trustframeworkkeyset"
}-->

```http
DELETE https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```
# <a name="c"></a>[<span data-ttu-id="63b2b-133">C#</span><span class="sxs-lookup"><span data-stu-id="63b2b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-trustframeworkkeyset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63b2b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63b2b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-trustframeworkkeyset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63b2b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63b2b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-trustframeworkkeyset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63b2b-136">Java</span><span class="sxs-lookup"><span data-stu-id="63b2b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-trustframeworkkeyset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="63b2b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="63b2b-137">Response</span></span>

<span data-ttu-id="63b2b-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="63b2b-138">The following is an example of the response.</span></span>

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


