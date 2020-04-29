---
title: Удаление Хомереалмдисковериполици
description: Удаление Хомереалмдисковериполици.
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8013887a3c34d0b58c2b0ad9b320586496f0dbda
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917128"
---
# <a name="delete-homerealmdiscoverypolicy"></a><span data-ttu-id="96b72-103">Удаление Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="96b72-103">Delete homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="96b72-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96b72-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="96b72-105">Удаление объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="96b72-105">Delete a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="96b72-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96b72-106">Permissions</span></span>

<span data-ttu-id="96b72-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96b72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96b72-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96b72-109">Permission type</span></span>                        | <span data-ttu-id="96b72-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96b72-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="96b72-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96b72-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="96b72-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="96b72-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="96b72-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96b72-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96b72-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96b72-114">Not supported.</span></span> |
| <span data-ttu-id="96b72-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96b72-115">Application</span></span>                            | <span data-ttu-id="96b72-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="96b72-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="96b72-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96b72-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="96b72-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96b72-118">Request headers</span></span>

| <span data-ttu-id="96b72-119">Имя</span><span class="sxs-lookup"><span data-stu-id="96b72-119">Name</span></span>          | <span data-ttu-id="96b72-120">Описание</span><span class="sxs-lookup"><span data-stu-id="96b72-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="96b72-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96b72-121">Authorization</span></span> | <span data-ttu-id="96b72-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96b72-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96b72-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="96b72-124">Request body</span></span>

<span data-ttu-id="96b72-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96b72-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96b72-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="96b72-126">Response</span></span>

<span data-ttu-id="96b72-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="96b72-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="96b72-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="96b72-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="96b72-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="96b72-129">Request</span></span>

<span data-ttu-id="96b72-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96b72-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="96b72-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="96b72-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="96b72-132">C#</span><span class="sxs-lookup"><span data-stu-id="96b72-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96b72-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96b72-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96b72-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96b72-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96b72-135">Java</span><span class="sxs-lookup"><span data-stu-id="96b72-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-homerealmdiscoverypolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="96b72-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="96b72-136">Response</span></span>

<span data-ttu-id="96b72-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="96b72-137">The following is an example of the response.</span></span>

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
  "description": "Delete homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
