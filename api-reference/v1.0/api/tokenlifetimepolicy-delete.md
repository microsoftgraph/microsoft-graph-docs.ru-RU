---
title: Удаление Токенлифетимеполици
description: Удаление Токенлифетимеполици.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bece069cb08e3eb909d2a10c0799729e08b3d673
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023033"
---
# <a name="delete-tokenlifetimepolicy"></a><span data-ttu-id="8f54f-103">Удаление Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="8f54f-103">Delete tokenLifetimePolicy</span></span>

<span data-ttu-id="8f54f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f54f-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="8f54f-105">Удаление объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8f54f-105">Delete a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f54f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f54f-106">Permissions</span></span>

<span data-ttu-id="8f54f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f54f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f54f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f54f-109">Permission type</span></span>                        | <span data-ttu-id="8f54f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f54f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8f54f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f54f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f54f-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8f54f-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="8f54f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f54f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f54f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f54f-114">Not supported.</span></span> |
| <span data-ttu-id="8f54f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8f54f-115">Application</span></span>                            | <span data-ttu-id="8f54f-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8f54f-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f54f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f54f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/tokenLifetimePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8f54f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f54f-118">Request headers</span></span>

| <span data-ttu-id="8f54f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8f54f-119">Name</span></span>          | <span data-ttu-id="8f54f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8f54f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8f54f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f54f-121">Authorization</span></span> | <span data-ttu-id="8f54f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f54f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f54f-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f54f-124">Request body</span></span>

<span data-ttu-id="8f54f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8f54f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f54f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f54f-126">Response</span></span>

<span data-ttu-id="8f54f-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8f54f-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8f54f-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="8f54f-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8f54f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f54f-129">Request</span></span>

<span data-ttu-id="8f54f-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f54f-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8f54f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8f54f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="8f54f-132">C#</span><span class="sxs-lookup"><span data-stu-id="8f54f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenlifetimepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8f54f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8f54f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenlifetimepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8f54f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8f54f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenlifetimepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8f54f-135">Java</span><span class="sxs-lookup"><span data-stu-id="8f54f-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tokenlifetimepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8f54f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f54f-136">Response</span></span>

<span data-ttu-id="8f54f-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8f54f-137">The following is an example of the response.</span></span>

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
  "description": "Delete tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

