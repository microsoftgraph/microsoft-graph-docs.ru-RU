---
title: 'appConsentRequest: filterByCurrentUser'
description: Извлечение объектов appConsentRequest, для которых текущий пользователь является рецензентом.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 47ebe3b69166ae7a8dc8d832a79ac86dfa09f15b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52750996"
---
# <a name="appconsentrequest-filterbycurrentuser"></a><span data-ttu-id="4a8f8-103">appConsentRequest: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="4a8f8-103">appConsentRequest: filterByCurrentUser</span></span>
<span data-ttu-id="4a8f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a8f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a8f8-105">Извлечение коллекции объектов [appConsentRequest,](../resources/appconsentrequest.md) для которых текущий пользователь является рецензентом, и состояние пользователяConsentRequest для доступа к указанному приложению `InProgress` .</span><span class="sxs-lookup"><span data-stu-id="4a8f8-105">Retrieve a collection of [appConsentRequest](../resources/appconsentrequest.md) objects for which the current user is the reviewer and the status of the userConsentRequest for accessing the specified app is `InProgress`.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a8f8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a8f8-106">Permissions</span></span>
<span data-ttu-id="4a8f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a8f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a8f8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a8f8-109">Permission type</span></span>|<span data-ttu-id="4a8f8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a8f8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a8f8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a8f8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4a8f8-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a8f8-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="4a8f8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a8f8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a8f8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a8f8-114">Not supported.</span></span>|
|<span data-ttu-id="4a8f8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="4a8f8-115">Application</span></span>|<span data-ttu-id="4a8f8-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a8f8-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a8f8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a8f8-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a><span data-ttu-id="4a8f8-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="4a8f8-118">Function parameters</span></span>
<span data-ttu-id="4a8f8-119">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="4a8f8-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="4a8f8-120">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="4a8f8-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4a8f8-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a8f8-121">Property</span></span>|<span data-ttu-id="4a8f8-122">Тип</span><span class="sxs-lookup"><span data-stu-id="4a8f8-122">Type</span></span>|<span data-ttu-id="4a8f8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4a8f8-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a8f8-124">on</span><span class="sxs-lookup"><span data-stu-id="4a8f8-124">on</span></span>|<span data-ttu-id="4a8f8-125">consentRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="4a8f8-125">consentRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="4a8f8-126">Фильтр для запроса объектов appConsentRequest, для которых текущий пользователь является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="4a8f8-126">Filter to query appConsentRequest objects for which the current user is a reviewer.</span></span> <span data-ttu-id="4a8f8-127">Разрешено значение `reviewer` .</span><span class="sxs-lookup"><span data-stu-id="4a8f8-127">Allowed value is `reviewer`.</span></span> <span data-ttu-id="4a8f8-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a8f8-128">Required.</span></span>|

## <a name="query-parameters"></a><span data-ttu-id="4a8f8-129">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="4a8f8-129">Query parameters</span></span>
<span data-ttu-id="4a8f8-130">Эта функция требует, чтобы параметр запроса OData возвращал коллекцию объектов  `$filter` [userConsentRequest,](../resources/userconsentrequest.md) для которых имеется `InProgress` состояние.</span><span class="sxs-lookup"><span data-stu-id="4a8f8-130">This function requires the `$filter` OData query parameter to return a collection of [userConsentRequest](../resources/userconsentrequest.md) objects for which the status is `InProgress`.</span></span> <span data-ttu-id="4a8f8-131">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4a8f8-131">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a8f8-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a8f8-132">Request headers</span></span>
|<span data-ttu-id="4a8f8-133">Имя</span><span class="sxs-lookup"><span data-stu-id="4a8f8-133">Name</span></span>|<span data-ttu-id="4a8f8-134">Описание</span><span class="sxs-lookup"><span data-stu-id="4a8f8-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4a8f8-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a8f8-135">Authorization</span></span>|<span data-ttu-id="4a8f8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a8f8-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a8f8-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a8f8-138">Request body</span></span>
<span data-ttu-id="4a8f8-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a8f8-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a8f8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a8f8-140">Response</span></span>

<span data-ttu-id="4a8f8-141">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [appConsentRequest](../resources/appconsentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4a8f8-141">If successful, this method returns a `200 OK` response code and a collection of [appConsentRequest](../resources/appconsentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a8f8-142">Пример</span><span class="sxs-lookup"><span data-stu-id="4a8f8-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a8f8-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a8f8-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4a8f8-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a8f8-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "appconsentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='reviewer')?$filter=userConsentRequests/any(u:u/status eq 'InProgress')
```
# <a name="c"></a>[<span data-ttu-id="4a8f8-145">C#</span><span class="sxs-lookup"><span data-stu-id="4a8f8-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/appconsentrequest-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a8f8-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a8f8-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/appconsentrequest-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a8f8-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a8f8-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/appconsentrequest-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a8f8-148">Java</span><span class="sxs-lookup"><span data-stu-id="4a8f8-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/appconsentrequest-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4a8f8-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a8f8-149">Response</span></span>
><span data-ttu-id="4a8f8-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4a8f8-150">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(appConsentRequest)",
  "@odata.count": 1,
  "value": [
    {
      "id": "af330b30-dd59-4482-a848-0fd81b0438ed",
      "appId": "3ca5f23f-94b4-4930-aec9-b8ca0f060e68",
      "appDisplayName": "Moodle",
      "consentType": "Dynamic",
      "pendingScopes": [],
      "userConsentRequests@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('af330b30-dd59-4482-a848-0fd81b0438ed')/userConsentRequests",
      "userConsentRequests": []
    }
  ]
}
```

