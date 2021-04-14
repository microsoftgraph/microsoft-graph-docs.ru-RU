---
title: 'appConsentRequest: filterByCurrentUser'
description: Извлечение объектов appConsentRequest, для которых текущий пользователь является рецензентом.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c17e44b27b135eec034eb66399d5ce5163a5928f
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697959"
---
# <a name="appconsentrequest-filterbycurrentuser"></a><span data-ttu-id="fef4f-103">appConsentRequest: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="fef4f-103">appConsentRequest: filterByCurrentUser</span></span>

<span data-ttu-id="fef4f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fef4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fef4f-105">Извлечение коллекции объектов [appConsentRequest,](../resources/appconsentrequest.md) для которых текущий пользователь является рецензентом, и состояние пользователяConsentRequest для доступа к указанному приложению `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="fef4f-105">Retrieve a collection of [appConsentRequest](../resources/appconsentrequest.md) objects for which the current user is the reviewer and the status of the userConsentRequest for accessing the specified app is `InProgress`.</span></span>

## <a name="permissions"></a><span data-ttu-id="fef4f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fef4f-106">Permissions</span></span>

<span data-ttu-id="fef4f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fef4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fef4f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fef4f-109">Permission type</span></span>|<span data-ttu-id="fef4f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fef4f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fef4f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fef4f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fef4f-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fef4f-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="fef4f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fef4f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fef4f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fef4f-114">Not supported.</span></span>|
|<span data-ttu-id="fef4f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fef4f-115">Application</span></span>|<span data-ttu-id="fef4f-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fef4f-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fef4f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fef4f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a><span data-ttu-id="fef4f-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="fef4f-118">Function parameters</span></span>

<span data-ttu-id="fef4f-119">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="fef4f-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="fef4f-120">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="fef4f-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="fef4f-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="fef4f-121">Parameter</span></span>|<span data-ttu-id="fef4f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="fef4f-122">Type</span></span>|<span data-ttu-id="fef4f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fef4f-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fef4f-124">on</span><span class="sxs-lookup"><span data-stu-id="fef4f-124">on</span></span>|<span data-ttu-id="fef4f-125">consentRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="fef4f-125">consentRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="fef4f-126">Фильтр для запроса объектов appConsentRequest, для которых текущий пользователь является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="fef4f-126">Filter to query appConsentRequest objects for which the current user is a reviewer.</span></span> <span data-ttu-id="fef4f-127">Разрешено значение `reviewer` .</span><span class="sxs-lookup"><span data-stu-id="fef4f-127">Allowed value is `reviewer`.</span></span> <span data-ttu-id="fef4f-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fef4f-128">Required.</span></span>|

## <a name="query-parameters"></a><span data-ttu-id="fef4f-129">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="fef4f-129">Query parameters</span></span>

<span data-ttu-id="fef4f-130">Эта функция требует, чтобы параметр запроса OData возвращал коллекцию объектов  `$filter` [userConsentRequest,](../resources/userconsentrequest.md) для которых имеется `InProgress` состояние.</span><span class="sxs-lookup"><span data-stu-id="fef4f-130">This function requires the `$filter` OData query parameter to return a collection of [userConsentRequest](../resources/userconsentrequest.md) objects for which the status is `InProgress`.</span></span> <span data-ttu-id="fef4f-131">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fef4f-131">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fef4f-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fef4f-132">Request headers</span></span>

|<span data-ttu-id="fef4f-133">Имя</span><span class="sxs-lookup"><span data-stu-id="fef4f-133">Name</span></span>|<span data-ttu-id="fef4f-134">Описание</span><span class="sxs-lookup"><span data-stu-id="fef4f-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fef4f-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fef4f-135">Authorization</span></span>|<span data-ttu-id="fef4f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fef4f-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fef4f-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fef4f-138">Request body</span></span>

<span data-ttu-id="fef4f-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fef4f-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fef4f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="fef4f-140">Response</span></span>

<span data-ttu-id="fef4f-141">В случае успеха эта функция возвращает код отклика и коллекцию объектов `200 OK` [appConsentRequest](../resources/appconsentrequest.md)  в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fef4f-141">If successful, this function returns a `200 OK` response code and a collection of [appConsentRequest](../resources/appconsentrequest.md)  objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fef4f-142">Пример</span><span class="sxs-lookup"><span data-stu-id="fef4f-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="fef4f-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="fef4f-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fef4f-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="fef4f-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "appconsentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='reviewer')?$filter=userConsentRequests/any(u:u/status eq 'InProgress')
```
# <a name="c"></a>[<span data-ttu-id="fef4f-145">C#</span><span class="sxs-lookup"><span data-stu-id="fef4f-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/appconsentrequest-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fef4f-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fef4f-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/appconsentrequest-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fef4f-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fef4f-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/appconsentrequest-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fef4f-148">Java</span><span class="sxs-lookup"><span data-stu-id="fef4f-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/appconsentrequest-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fef4f-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="fef4f-149">Response</span></span>

<span data-ttu-id="fef4f-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fef4f-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.appConsentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(appConsentRequest)",
  "@odata.count": 1,
  "value": [
    {
      "id": "af330b30-dd59-4482-a848-0fd81b0438ed",
      "appId": "3ca5f23f-94b4-4930-aec9-b8ca0f060e68",
      "appDisplayName": "Moodle",
      "pendingScopes": [],
      "userConsentRequests@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('af330b30-dd59-4482-a848-0fd81b0438ed')/userConsentRequests",
      "userConsentRequests": []
    }
  ]
}
```

