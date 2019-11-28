---
title: Удаление Намедлокатион
description: Удаление объекта Намедлокатион.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dbe72bf1024647467fc7df2f54ce5f15cacdfad5
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636843"
---
# <a name="delete-namedlocation"></a><span data-ttu-id="eea52-103">Удаление Намедлокатион</span><span class="sxs-lookup"><span data-stu-id="eea52-103">Delete namedLocation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eea52-104">Удаление объекта [намедлокатион](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="eea52-104">Delete a [namedLocation](../resources/namedlocation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="eea52-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eea52-105">Permissions</span></span>

<span data-ttu-id="eea52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eea52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eea52-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eea52-108">Permission type</span></span>                        | <span data-ttu-id="eea52-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eea52-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="eea52-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eea52-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="eea52-111">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="eea52-111">Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="eea52-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eea52-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eea52-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eea52-113">Not supported.</span></span> |
| <span data-ttu-id="eea52-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eea52-114">Application</span></span>                            | <span data-ttu-id="eea52-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eea52-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eea52-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eea52-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="eea52-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eea52-117">Request headers</span></span>

| <span data-ttu-id="eea52-118">Имя</span><span class="sxs-lookup"><span data-stu-id="eea52-118">Name</span></span>          | <span data-ttu-id="eea52-119">Описание</span><span class="sxs-lookup"><span data-stu-id="eea52-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="eea52-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eea52-120">Authorization</span></span> | <span data-ttu-id="eea52-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eea52-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eea52-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eea52-123">Request body</span></span>

<span data-ttu-id="eea52-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eea52-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eea52-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="eea52-125">Response</span></span>

<span data-ttu-id="eea52-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="eea52-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eea52-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="eea52-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eea52-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="eea52-129">Request</span></span>

<span data-ttu-id="eea52-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eea52-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="eea52-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="eea52-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_namedlocation"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="eea52-132">C#</span><span class="sxs-lookup"><span data-stu-id="eea52-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-namedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eea52-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eea52-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-namedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eea52-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eea52-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-namedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eea52-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="eea52-135">Response</span></span>

<span data-ttu-id="eea52-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="eea52-136">The following is an example of the response.</span></span>

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
