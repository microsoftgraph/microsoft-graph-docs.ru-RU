---
title: Удаление Хомереалмдисковериполици
description: Удаление Хомереалмдисковериполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 363e1101686d2e5cb5d6b9df452cf6ef700f5dbd
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805616"
---
# <a name="delete-homerealmdiscoverypolicy"></a><span data-ttu-id="47efd-103">Удаление Хомереалмдисковериполици</span><span class="sxs-lookup"><span data-stu-id="47efd-103">Delete homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="47efd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47efd-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="47efd-105">Удаление объекта [хомереалмдисковериполици](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="47efd-105">Delete a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="47efd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47efd-106">Permissions</span></span>

<span data-ttu-id="47efd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47efd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="47efd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47efd-109">Permission type</span></span>                        | <span data-ttu-id="47efd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47efd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="47efd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47efd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="47efd-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="47efd-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="47efd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47efd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47efd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47efd-114">Not supported.</span></span> |
| <span data-ttu-id="47efd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47efd-115">Application</span></span>                            | <span data-ttu-id="47efd-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="47efd-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="47efd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47efd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="47efd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47efd-118">Request headers</span></span>

| <span data-ttu-id="47efd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="47efd-119">Name</span></span>          | <span data-ttu-id="47efd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="47efd-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="47efd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47efd-121">Authorization</span></span> | <span data-ttu-id="47efd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47efd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47efd-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47efd-124">Request body</span></span>

<span data-ttu-id="47efd-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47efd-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47efd-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="47efd-126">Response</span></span>

<span data-ttu-id="47efd-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="47efd-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="47efd-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="47efd-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47efd-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="47efd-129">Request</span></span>

<span data-ttu-id="47efd-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47efd-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="47efd-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="47efd-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="47efd-132">C#</span><span class="sxs-lookup"><span data-stu-id="47efd-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47efd-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47efd-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47efd-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47efd-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47efd-135">Java</span><span class="sxs-lookup"><span data-stu-id="47efd-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-homerealmdiscoverypolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="47efd-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="47efd-136">Response</span></span>

<span data-ttu-id="47efd-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="47efd-137">The following is an example of the response.</span></span>

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
