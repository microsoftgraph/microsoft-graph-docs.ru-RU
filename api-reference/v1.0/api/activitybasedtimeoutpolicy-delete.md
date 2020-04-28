---
title: Удаление Активитибаседтимеаутполици
description: Удаление Активитибаседтимеаутполици.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ee3ed0c1abd7c1e392bbed47e5fba568506be1b
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917106"
---
# <a name="delete-activitybasedtimeoutpolicy"></a><span data-ttu-id="14b99-103">Удаление Активитибаседтимеаутполици</span><span class="sxs-lookup"><span data-stu-id="14b99-103">Delete activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="14b99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14b99-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="14b99-105">Удаление объекта [активитибаседтимеаутполици](../resources/activitybasedtimeoutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="14b99-105">Delete an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="14b99-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14b99-106">Permissions</span></span>

<span data-ttu-id="14b99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14b99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14b99-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14b99-109">Permission type</span></span>                        | <span data-ttu-id="14b99-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14b99-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="14b99-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14b99-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="14b99-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="14b99-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="14b99-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14b99-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14b99-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14b99-114">Not supported.</span></span> |
| <span data-ttu-id="14b99-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14b99-115">Application</span></span>                            | <span data-ttu-id="14b99-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="14b99-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="14b99-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14b99-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="14b99-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14b99-118">Request headers</span></span>

| <span data-ttu-id="14b99-119">Имя</span><span class="sxs-lookup"><span data-stu-id="14b99-119">Name</span></span>          | <span data-ttu-id="14b99-120">Описание</span><span class="sxs-lookup"><span data-stu-id="14b99-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="14b99-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14b99-121">Authorization</span></span> | <span data-ttu-id="14b99-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14b99-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14b99-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14b99-124">Request body</span></span>

<span data-ttu-id="14b99-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="14b99-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14b99-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="14b99-126">Response</span></span>

<span data-ttu-id="14b99-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="14b99-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="14b99-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="14b99-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14b99-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="14b99-129">Request</span></span>

<span data-ttu-id="14b99-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14b99-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="14b99-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="14b99-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_activitybasedtimeoutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="14b99-132">C#</span><span class="sxs-lookup"><span data-stu-id="14b99-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14b99-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14b99-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14b99-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14b99-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14b99-135">Java</span><span class="sxs-lookup"><span data-stu-id="14b99-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-activitybasedtimeoutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14b99-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="14b99-136">Response</span></span>

<span data-ttu-id="14b99-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="14b99-137">The following is an example of the response.</span></span>

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
  "description": "Delete activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
