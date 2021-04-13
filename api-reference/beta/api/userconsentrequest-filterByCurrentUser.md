---
title: 'userConsentRequest: filterByCurrentUser'
description: Извлечение объектов userConsentRequest, для которых текущий пользователь является рецензентом.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 939e0c113f2ff5935c89530b304c3ad95b4e46e7
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2021
ms.locfileid: "51698092"
---
# <a name="userconsentrequest-filterbycurrentuser"></a><span data-ttu-id="5c748-103">userConsentRequest: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="5c748-103">userConsentRequest: filterByCurrentUser</span></span>
<span data-ttu-id="5c748-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c748-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c748-105">Извлечение коллекции [объектов userConsentRequest](../resources/userconsentrequest.md) для доступа к указанному приложению, для которого текущий пользователь является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="5c748-105">Retrieve a collection of [userConsentRequest](../resources/userconsentrequest.md) objects for accessing a specified app, for which the current user is the reviewer.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c748-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c748-106">Permissions</span></span>
<span data-ttu-id="5c748-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c748-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c748-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c748-109">Permission type</span></span>|<span data-ttu-id="5c748-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c748-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c748-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c748-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c748-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c748-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="5c748-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c748-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c748-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c748-114">Not supported.</span></span>|
|<span data-ttu-id="5c748-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c748-115">Application</span></span>|<span data-ttu-id="5c748-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c748-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c748-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c748-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{id}/userConsentRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a><span data-ttu-id="5c748-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="5c748-118">Function parameters</span></span>
<span data-ttu-id="5c748-119">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="5c748-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="5c748-120">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="5c748-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="5c748-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c748-121">Property</span></span>|<span data-ttu-id="5c748-122">Тип</span><span class="sxs-lookup"><span data-stu-id="5c748-122">Type</span></span>|<span data-ttu-id="5c748-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5c748-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c748-124">on</span><span class="sxs-lookup"><span data-stu-id="5c748-124">on</span></span>|<span data-ttu-id="5c748-125">consentRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="5c748-125">consentRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="5c748-126">Фильтр для запроса объектов userConsentRequest для объекта appConsentRequest, для которого текущий пользователь является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="5c748-126">Filter to query userConsentRequest objects for an appConsentRequest object for which the current user is a reviewer.</span></span> <span data-ttu-id="5c748-127">Разрешено значение `reviewer` .</span><span class="sxs-lookup"><span data-stu-id="5c748-127">Allowed value is `reviewer`.</span></span> <span data-ttu-id="5c748-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c748-128">Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="5c748-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5c748-129">Optional query parameters</span></span>
<span data-ttu-id="5c748-130">Эта функция поддерживает параметр  `$filter` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5c748-130">This function supports the `$filter` OData query parameter to help customize the response.</span></span> <span data-ttu-id="5c748-131">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5c748-131">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c748-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c748-132">Request headers</span></span>
|<span data-ttu-id="5c748-133">Имя</span><span class="sxs-lookup"><span data-stu-id="5c748-133">Name</span></span>|<span data-ttu-id="5c748-134">Описание</span><span class="sxs-lookup"><span data-stu-id="5c748-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5c748-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c748-135">Authorization</span></span>|<span data-ttu-id="5c748-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c748-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c748-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c748-138">Request body</span></span>
<span data-ttu-id="5c748-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c748-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c748-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c748-140">Response</span></span>

<span data-ttu-id="5c748-141">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [userConsentRequest](../resources/userconsentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5c748-141">If successful, this method returns a `200 OK` response code and a collection of [userConsentRequest](../resources/userconsentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c748-142">Пример</span><span class="sxs-lookup"><span data-stu-id="5c748-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c748-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c748-143">Request</span></span>

<span data-ttu-id="5c748-144">В этом запросе вы перечислите все **объекты userConsentRequest,** для которых текущий пользователь является рецензентом и состояние `Completed` .</span><span class="sxs-lookup"><span data-stu-id="5c748-144">In this request, you list all **userConsentRequest** objects for which the current user is the reviewer and the status is `Completed`.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c748-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c748-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "userconsentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests/filterByCurrentUser(on='reviewer')?$filter= (status eq 'Completed')
```
# <a name="c"></a>[<span data-ttu-id="5c748-146">C#</span><span class="sxs-lookup"><span data-stu-id="5c748-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/userconsentrequest-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c748-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c748-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/userconsentrequest-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c748-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c748-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/userconsentrequest-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c748-149">Java</span><span class="sxs-lookup"><span data-stu-id="5c748-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/userconsentrequest-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5c748-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c748-150">Response</span></span>
<span data-ttu-id="5c748-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5c748-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userConsentRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userConsentRequest)",
    "@odata.count": 1,
    "value": [
      {
      "id": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
      "reason": "I need access",
      "status": "Completed",
      "createdDateTime": "2019-10-18T19:07:19.7374554Z",
      "createdBy": {
        "user": {
          "id": "db60ab61-caea-4889-a824-98de31ef31b5",
          "displayName": "Alex Wilber",
          "userPrincipalName": "AlexW@contoso.com",
          "mail": "AlexW@contoso.com"
        }
      },
      "approval@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests('acef2660-d194-4943-b927-4fe4fb5cb7e3')/approval/$entity",
      "approval": {
        "id": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
        "steps@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests('acef2660-d194-4943-b927-4fe4fb5cb7e3')/approval/steps",
        "steps": [
          {
            "id": "f5a4ca4a-1316-4872-8112-993c55dab51e",
            "displayName": null,
            "reviewedDateTime": "2019-10-19T04:12:09.633Z",
            "reviewResult": "Approve",
            "status": "Completed",
            "assignedToMe": true,
            "justification": "Admin consent granted.",
            "reviewedBy": {
              "id": "00000001-0000-0000-c000-000000000000",
              "displayName": "",
              "userPrincipalName": "",
              "mail": ""
            }
          }
        ]
      },
      "approvalId": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
      "completedDateTime": null,
      "customData": null
    }
  ]
}
```
