---
title: Удаление пользовательского потока
description: Удаление пользовательского потока.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6185c79777772b461c562f831d1bb135f2a00aa0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435352"
---
# <a name="delete-userflow"></a><span data-ttu-id="265ed-103">Удаление пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="265ed-103">Delete userFlow</span></span>

<span data-ttu-id="265ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="265ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="265ed-105">Удаление существующего [объекта пользовательского потока.](../resources/identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="265ed-105">Delete an existing [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="265ed-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="265ed-106">Permissions</span></span>

<span data-ttu-id="265ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="265ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="265ed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="265ed-109">Permission type</span></span>                        | <span data-ttu-id="265ed-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="265ed-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="265ed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="265ed-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="265ed-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="265ed-112">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="265ed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="265ed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="265ed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="265ed-114">Not supported.</span></span> |
| <span data-ttu-id="265ed-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="265ed-115">Application</span></span>                            | <span data-ttu-id="265ed-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="265ed-116">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="265ed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="265ed-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="265ed-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="265ed-118">Request headers</span></span>

| <span data-ttu-id="265ed-119">Имя</span><span class="sxs-lookup"><span data-stu-id="265ed-119">Name</span></span>          | <span data-ttu-id="265ed-120">Описание</span><span class="sxs-lookup"><span data-stu-id="265ed-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="265ed-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="265ed-121">Authorization</span></span> | <span data-ttu-id="265ed-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="265ed-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="265ed-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="265ed-124">Request body</span></span>

<span data-ttu-id="265ed-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="265ed-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="265ed-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="265ed-126">Response</span></span>

<span data-ttu-id="265ed-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="265ed-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="265ed-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="265ed-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="265ed-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="265ed-130">Request</span></span>

<span data-ttu-id="265ed-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="265ed-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="265ed-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="265ed-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityuserflow"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/userFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="265ed-133">C#</span><span class="sxs-lookup"><span data-stu-id="265ed-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="265ed-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="265ed-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="265ed-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="265ed-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="265ed-136">Java</span><span class="sxs-lookup"><span data-stu-id="265ed-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="265ed-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="265ed-137">Response</span></span>

<span data-ttu-id="265ed-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="265ed-138">The following is an example of the response.</span></span>

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
  "description": "Delete userFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


