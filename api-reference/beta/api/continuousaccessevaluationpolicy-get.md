---
title: Get continuousAccessEvaluationPolicy
description: Ознакомьтесь с свойствами объекта continuousAccessEvaluationPolicy.
author: jerrysai
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0f0aac891c40e84266ebb48fb3e196bbdfd13d03
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437291"
---
# <a name="get-continuousaccessevaluationpolicy"></a><span data-ttu-id="f2608-103">Get continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="f2608-103">Get continuousAccessEvaluationPolicy</span></span>
<span data-ttu-id="f2608-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2608-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2608-105">Ознакомьтесь с свойствами и отношениями объекта [continuousAccessEvaluationPolicy.](../resources/continuousaccessevaluationpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f2608-105">Read the properties and relationships of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2608-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2608-106">Permissions</span></span>
<span data-ttu-id="f2608-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2608-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2608-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2608-109">Permission type</span></span>|<span data-ttu-id="f2608-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2608-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2608-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2608-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2608-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2608-112">Policy.Read.All</span></span> |
|<span data-ttu-id="f2608-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2608-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2608-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2608-114">Not supported.</span></span> |
|<span data-ttu-id="f2608-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2608-115">Application</span></span>                            | <span data-ttu-id="f2608-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2608-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2608-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2608-117">HTTP request</span></span>

<!-- {  "blockType": "ignored"} -->
``` http
GET /identity/continuousAccessEvaluationPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2608-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f2608-118">Optional query parameters</span></span>
<span data-ttu-id="f2608-119">Этот метод поддерживает параметр запроса $select OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f2608-119">This method supports the '$select' OData query parameter to help customize the response.</span></span> <span data-ttu-id="f2608-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f2608-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2608-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2608-121">Request headers</span></span>
|<span data-ttu-id="f2608-122">Имя</span><span class="sxs-lookup"><span data-stu-id="f2608-122">Name</span></span>|<span data-ttu-id="f2608-123">Описание</span><span class="sxs-lookup"><span data-stu-id="f2608-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f2608-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2608-124">Authorization</span></span>|<span data-ttu-id="f2608-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2608-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2608-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f2608-127">Request body</span></span>
<span data-ttu-id="f2608-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2608-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2608-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2608-129">Response</span></span>

<span data-ttu-id="f2608-130">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f2608-130">If successful, this method returns a `200 OK` response code and a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f2608-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="f2608-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2608-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2608-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f2608-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2608-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_continuousaccessevaluationpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/continuousAccessEvaluationPolicy
```
# <a name="c"></a>[<span data-ttu-id="f2608-134">C#</span><span class="sxs-lookup"><span data-stu-id="f2608-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-continuousaccessevaluationpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2608-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2608-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-continuousaccessevaluationpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2608-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2608-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-continuousaccessevaluationpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2608-137">Java</span><span class="sxs-lookup"><span data-stu-id="f2608-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-continuousaccessevaluationpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f2608-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2608-138">Response</span></span>

<span data-ttu-id="f2608-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f2608-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.continuousAccessEvaluationPolicy"
} -->

``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/continuousAccessEvaluationPolicy/$entity",
  "id": "00000000-0000-0000-0000-000000000006",
  "description": "Continuous Access Evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.",
  "displayName": "Continuous Access Evaluation",
  "isEnabled": true,
  "users": [ "1608be63-df14-42a4-8932-1c9d963b026f" ],
  "groups": [ "4308b567-df14-0000-8932-1c9d963b026f" ]
}
```
