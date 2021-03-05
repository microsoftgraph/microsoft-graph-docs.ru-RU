---
title: Удаление namedLocation
description: Удаление объекта namedLocation.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6a51da64e4e04d962991303d2cd23f5a4f71372a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448237"
---
# <a name="delete-namedlocation"></a><span data-ttu-id="925cc-103">Удаление namedLocation</span><span class="sxs-lookup"><span data-stu-id="925cc-103">Delete namedLocation</span></span>

<span data-ttu-id="925cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="925cc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="925cc-105">Удаление [объекта namedLocation.](../resources/namedlocation.md)</span><span class="sxs-lookup"><span data-stu-id="925cc-105">Delete a [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="925cc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="925cc-106">Permissions</span></span>

<span data-ttu-id="925cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="925cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="925cc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="925cc-109">Permission type</span></span>                        | <span data-ttu-id="925cc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="925cc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="925cc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="925cc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="925cc-112">Policy.Read.All и Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="925cc-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="925cc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="925cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="925cc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="925cc-114">Not supported.</span></span> |
| <span data-ttu-id="925cc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="925cc-115">Application</span></span>                            | <span data-ttu-id="925cc-116">Policy.Read.All и Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="925cc-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="925cc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="925cc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="925cc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="925cc-118">Request headers</span></span>

| <span data-ttu-id="925cc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="925cc-119">Name</span></span>          | <span data-ttu-id="925cc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="925cc-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="925cc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="925cc-121">Authorization</span></span> | <span data-ttu-id="925cc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="925cc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="925cc-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="925cc-124">Request body</span></span>

<span data-ttu-id="925cc-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="925cc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="925cc-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="925cc-126">Response</span></span>

<span data-ttu-id="925cc-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="925cc-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="925cc-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="925cc-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="925cc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="925cc-130">Request</span></span>

<span data-ttu-id="925cc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="925cc-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="925cc-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="925cc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_namedlocation"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="c"></a>[<span data-ttu-id="925cc-133">C#</span><span class="sxs-lookup"><span data-stu-id="925cc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-namedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="925cc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="925cc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-namedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="925cc-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="925cc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-namedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="925cc-136">Java</span><span class="sxs-lookup"><span data-stu-id="925cc-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-namedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="925cc-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="925cc-137">Response</span></span>

<span data-ttu-id="925cc-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="925cc-138">The following is an example of the response.</span></span>

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
  "description": "Delete namedLocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

