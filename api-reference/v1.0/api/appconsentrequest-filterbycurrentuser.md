---
title: 'appConsentRequest: filterByCurrentUser'
description: Извлечение appConsentRequests, для которых текущий пользователь является рецензентом.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b87e79923b0ea22b9ac32c465885a1f9e259a47f
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469642"
---
# <a name="appconsentrequest-filterbycurrentuser"></a><span data-ttu-id="a9406-103">appConsentRequest: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="a9406-103">appConsentRequest: filterByCurrentUser</span></span>

<span data-ttu-id="a9406-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9406-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a9406-105">Извлечения [appConsentRequests,](../resources/appconsentrequest.md) для которых текущий пользователь является рецензентом и состояние userConsentRequest `InProgress` является .</span><span class="sxs-lookup"><span data-stu-id="a9406-105">Retrieve [appConsentRequests](../resources/appconsentrequest.md) for which the current user is the reviewer and the status of the userConsentRequest is `InProgress`.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9406-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9406-106">Permissions</span></span>

<span data-ttu-id="a9406-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9406-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9406-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9406-109">Permission type</span></span>|<span data-ttu-id="a9406-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9406-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9406-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9406-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a9406-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9406-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="a9406-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9406-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9406-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9406-114">Not supported.</span></span>|
|<span data-ttu-id="a9406-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9406-115">Application</span></span>|<span data-ttu-id="a9406-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9406-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9406-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9406-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a><span data-ttu-id="a9406-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="a9406-118">Function parameters</span></span>

<span data-ttu-id="a9406-119">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="a9406-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="a9406-120">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="a9406-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a9406-121">Параметр</span><span class="sxs-lookup"><span data-stu-id="a9406-121">Parameter</span></span>|<span data-ttu-id="a9406-122">Тип</span><span class="sxs-lookup"><span data-stu-id="a9406-122">Type</span></span>|<span data-ttu-id="a9406-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a9406-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9406-124">on</span><span class="sxs-lookup"><span data-stu-id="a9406-124">on</span></span>|<span data-ttu-id="a9406-125">consentRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="a9406-125">consentRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="a9406-126">Фильтр для запроса appConsentRequests, для которого текущий пользователь является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="a9406-126">Filter to query appConsentRequests for which the current user is a reviewer.</span></span> <span data-ttu-id="a9406-127">Разрешено значение `reviewer` .</span><span class="sxs-lookup"><span data-stu-id="a9406-127">Allowed value is `reviewer`.</span></span> <span data-ttu-id="a9406-128">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="a9406-128">Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="a9406-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a9406-129">Optional query parameters</span></span>

<span data-ttu-id="a9406-130">Эта функция требует, чтобы параметр запроса OData возвращал коллекцию  `$filter` [userConsentRequests,](../resources/userconsentrequest.md) для которых имеется `InProgress` состояние.</span><span class="sxs-lookup"><span data-stu-id="a9406-130">This function requires the `$filter` OData query parameter to return a collection of [userConsentRequests](../resources/userconsentrequest.md) for which the status is `InProgress`.</span></span> <span data-ttu-id="a9406-131">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a9406-131">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9406-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9406-132">Request headers</span></span>

|<span data-ttu-id="a9406-133">Имя</span><span class="sxs-lookup"><span data-stu-id="a9406-133">Name</span></span>|<span data-ttu-id="a9406-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a9406-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a9406-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9406-135">Authorization</span></span>|<span data-ttu-id="a9406-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9406-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9406-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9406-138">Request body</span></span>

<span data-ttu-id="a9406-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a9406-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9406-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9406-140">Response</span></span>

<span data-ttu-id="a9406-141">В случае успешной работы эта функция возвращает код отклика и `200 OK` [коллекцию appConsentRequest](../resources/appconsentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a9406-141">If successful, this function returns a `200 OK` response code and a [appConsentRequest](../resources/appconsentrequest.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a9406-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="a9406-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a9406-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9406-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "appconsentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/appConsent/appConsentRequests/filterByCurrentUser(on='reviewer')?$filter=userConsentRequests/any(u:u/status eq 'InProgress')
```

### <a name="response"></a><span data-ttu-id="a9406-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9406-144">Response</span></span>

<span data-ttu-id="a9406-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a9406-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "consentType": "Dynamic",
      "userConsentRequests@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('af330b30-dd59-4482-a848-0fd81b0438ed')/userConsentRequests",
      "userConsentRequests": []
    }
  ]
}
```

