---
title: Получить accessReviewPolicy
description: Ознакомьтесь с свойствами и отношениями объекта accessReviewPolicy.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c2acf367b269e47271e3f3629ed05ce283201c1c
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241008"
---
# <a name="get-accessreviewpolicy"></a><span data-ttu-id="57d3c-103">Получить accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="57d3c-103">Get accessReviewPolicy</span></span>
<span data-ttu-id="57d3c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57d3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57d3c-105">Ознакомьтесь с свойствами и отношениями [объекта accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="57d3c-105">Read the properties and relationships of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="57d3c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57d3c-106">Permissions</span></span>
<span data-ttu-id="57d3c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57d3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57d3c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57d3c-109">Permission type</span></span>|<span data-ttu-id="57d3c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57d3c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57d3c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57d3c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="57d3c-112">Policy.Read.All, Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="57d3c-112">Policy.Read.All, Policy.ReadWrite.AccessReviews</span></span>|
|<span data-ttu-id="57d3c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57d3c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57d3c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57d3c-114">Not supported.</span></span>|
|<span data-ttu-id="57d3c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57d3c-115">Application</span></span>|<span data-ttu-id="57d3c-116">Policy.Read.All, Policy.ReadWrite.AccessReviews</span><span class="sxs-lookup"><span data-stu-id="57d3c-116">Policy.Read.All, Policy.ReadWrite.AccessReviews</span></span>|

## <a name="http-request"></a><span data-ttu-id="57d3c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57d3c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/accessReviewPolicy
GET /identityGovernance/accessReviews/policy
```

## <a name="request-headers"></a><span data-ttu-id="57d3c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57d3c-118">Request headers</span></span>
|<span data-ttu-id="57d3c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="57d3c-119">Name</span></span>|<span data-ttu-id="57d3c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="57d3c-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="57d3c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57d3c-121">Authorization</span></span>|<span data-ttu-id="57d3c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57d3c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57d3c-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57d3c-124">Request body</span></span>
<span data-ttu-id="57d3c-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57d3c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57d3c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="57d3c-126">Response</span></span>

<span data-ttu-id="57d3c-127">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект accessReviewPolicy](../resources/accessreviewpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="57d3c-127">If successful, this method returns a `200 OK` response code and an [accessReviewPolicy](../resources/accessreviewpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57d3c-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="57d3c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="57d3c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="57d3c-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="57d3c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="57d3c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/accessReviewPolicy
```
# <a name="c"></a>[<span data-ttu-id="57d3c-131">C#</span><span class="sxs-lookup"><span data-stu-id="57d3c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57d3c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57d3c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57d3c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57d3c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57d3c-134">Java</span><span class="sxs-lookup"><span data-stu-id="57d3c-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="57d3c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="57d3c-135">Response</span></span>
<span data-ttu-id="57d3c-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="57d3c-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewPolicy",
    "displayName": "Access Review Policy",
    "description": "Policy contains directory-level access review settings.",
    "isGroupOwnerManagementEnabled": false
  }
}
```

### <a name="request"></a><span data-ttu-id="57d3c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="57d3c-137">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="57d3c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="57d3c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewpolicy_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/policy
```
# <a name="c"></a>[<span data-ttu-id="57d3c-139">C#</span><span class="sxs-lookup"><span data-stu-id="57d3c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewpolicy-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57d3c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57d3c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewpolicy-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57d3c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57d3c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewpolicy-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57d3c-142">Java</span><span class="sxs-lookup"><span data-stu-id="57d3c-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewpolicy-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="57d3c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="57d3c-143">Response</span></span>
<span data-ttu-id="57d3c-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="57d3c-144">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.accessReviewPolicy",
    "displayName": "Access Review Policy",
    "description": "Policy contains directory-level access review settings.",
    "isGroupOwnerManagementEnabled": false
  }
}
```
