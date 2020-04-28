---
title: Удаление Токенлифетимеполици
description: Удаление Токенлифетимеполици.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 930219215c38b0e0252b84f5e8168ece8429e65b
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917445"
---
# <a name="delete-tokenlifetimepolicy"></a><span data-ttu-id="6c84e-103">Удаление Токенлифетимеполици</span><span class="sxs-lookup"><span data-stu-id="6c84e-103">Delete tokenLifetimePolicy</span></span>

<span data-ttu-id="6c84e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c84e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c84e-105">Удаление объекта [токенлифетимеполици](../resources/tokenlifetimepolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="6c84e-105">Delete a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c84e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6c84e-106">Permissions</span></span>

<span data-ttu-id="6c84e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c84e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c84e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c84e-109">Permission type</span></span>                        | <span data-ttu-id="6c84e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c84e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6c84e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c84e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c84e-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c84e-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="6c84e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c84e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c84e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c84e-114">Not supported.</span></span> |
| <span data-ttu-id="6c84e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6c84e-115">Application</span></span>                            | <span data-ttu-id="6c84e-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c84e-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c84e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c84e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/tokenLifetimePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6c84e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6c84e-118">Request headers</span></span>

| <span data-ttu-id="6c84e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6c84e-119">Name</span></span>          | <span data-ttu-id="6c84e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6c84e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6c84e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6c84e-121">Authorization</span></span> | <span data-ttu-id="6c84e-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6c84e-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c84e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c84e-123">Request body</span></span>

<span data-ttu-id="6c84e-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c84e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c84e-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c84e-125">Response</span></span>

<span data-ttu-id="6c84e-126">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6c84e-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6c84e-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="6c84e-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c84e-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c84e-128">Request</span></span>

<span data-ttu-id="6c84e-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c84e-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6c84e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c84e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="6c84e-131">C#</span><span class="sxs-lookup"><span data-stu-id="6c84e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenlifetimepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c84e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c84e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenlifetimepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c84e-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c84e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenlifetimepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6c84e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c84e-134">Response</span></span>

<span data-ttu-id="6c84e-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6c84e-135">The following is an example of the response.</span></span>

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
