---
title: 'userConsentRequests: filterByCurrentUser'
description: Извлечение userConsentRequests, для которых текущий пользователь является рецензентом.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a4fe32aab22b425fcdf58389bc6b71cae2147b42
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965140"
---
# <a name="userconsentrequests-filterbycurrentuser"></a><span data-ttu-id="1fd9d-103">userConsentRequests: filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="1fd9d-103">userConsentRequests: filterByCurrentUser</span></span>
<span data-ttu-id="1fd9d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fd9d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fd9d-105">Извлечения [userConsentRequests](../resources/userconsentrequest.md) для appConsentRequest, для которого текущий пользователь является рецензентом и состояние userConsentRequest `InProgress` является .</span><span class="sxs-lookup"><span data-stu-id="1fd9d-105">Retrieve the [userConsentRequests](../resources/userconsentrequest.md) for an appConsentRequest for which the current user is the reviewer and the status of the userConsentRequest is `InProgress`.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fd9d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1fd9d-106">Permissions</span></span>
<span data-ttu-id="1fd9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fd9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fd9d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fd9d-109">Permission type</span></span>|<span data-ttu-id="1fd9d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fd9d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fd9d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fd9d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1fd9d-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fd9d-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="1fd9d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fd9d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fd9d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fd9d-114">Not supported.</span></span>|
|<span data-ttu-id="1fd9d-115">Application</span><span class="sxs-lookup"><span data-stu-id="1fd9d-115">Application</span></span>|<span data-ttu-id="1fd9d-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fd9d-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fd9d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fd9d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{id}/userConsentRequests/filterByCurrentUser(on='parameterValue')
```

## <a name="function-parameters"></a><span data-ttu-id="1fd9d-118">Параметры функции</span><span class="sxs-lookup"><span data-stu-id="1fd9d-118">Function parameters</span></span>
<span data-ttu-id="1fd9d-119">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="1fd9d-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="1fd9d-120">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="1fd9d-120">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="1fd9d-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="1fd9d-121">Property</span></span>|<span data-ttu-id="1fd9d-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1fd9d-122">Type</span></span>|<span data-ttu-id="1fd9d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1fd9d-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fd9d-124">on</span><span class="sxs-lookup"><span data-stu-id="1fd9d-124">on</span></span>|<span data-ttu-id="1fd9d-125">consentRequestFilterByCurrentUserOptions</span><span class="sxs-lookup"><span data-stu-id="1fd9d-125">consentRequestFilterByCurrentUserOptions</span></span>|<span data-ttu-id="1fd9d-126">Фильтр для запроса userConsentRequests для приложенияConsentRequest, для которого текущий пользователь является рецензентом.</span><span class="sxs-lookup"><span data-stu-id="1fd9d-126">Filter to query userConsentRequests for an appConsentRequest for which the current user is a reviewer.</span></span> <span data-ttu-id="1fd9d-127">Разрешено значение `reviewer` .</span><span class="sxs-lookup"><span data-stu-id="1fd9d-127">Allowed value is `reviewer`.</span></span> <span data-ttu-id="1fd9d-128">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fd9d-128">Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="1fd9d-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1fd9d-129">Optional query parameters</span></span>
<span data-ttu-id="1fd9d-130">Эта функция поддерживает параметр  `$filter` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1fd9d-130">This function supports the `$filter` OData query parameter to help customize the response.</span></span> <span data-ttu-id="1fd9d-131">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1fd9d-131">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1fd9d-132">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1fd9d-132">Request headers</span></span>
|<span data-ttu-id="1fd9d-133">Имя</span><span class="sxs-lookup"><span data-stu-id="1fd9d-133">Name</span></span>|<span data-ttu-id="1fd9d-134">Описание</span><span class="sxs-lookup"><span data-stu-id="1fd9d-134">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1fd9d-135">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1fd9d-135">Authorization</span></span>|<span data-ttu-id="1fd9d-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fd9d-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fd9d-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1fd9d-138">Request body</span></span>
<span data-ttu-id="1fd9d-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1fd9d-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fd9d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fd9d-140">Response</span></span>

<span data-ttu-id="1fd9d-141">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [userConsentRequest](../resources/userconsentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1fd9d-141">If successful, this method returns a `200 OK` response code and a collection of [userConsentRequest](../resources/userconsentrequest.md) objects in the response body.</span></span>

## <a name="example-list-all-userconsentrequests-for-which-the-current-user-is-the-reviewer-and-the-status-is-completed"></a><span data-ttu-id="1fd9d-142">Пример. Список всех userConsentRequests, для которых текущий пользователь является рецензентом и состояние завершено</span><span class="sxs-lookup"><span data-stu-id="1fd9d-142">Example: List all userConsentRequests for which the current user is the reviewer and the status is Completed</span></span>

### <a name="request"></a><span data-ttu-id="1fd9d-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fd9d-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "userconsentrequest_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests/filterByCurrentUser(on='reviewer')?$filter= (status eq 'Completed')
```


### <a name="response"></a><span data-ttu-id="1fd9d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fd9d-144">Response</span></span>
<span data-ttu-id="1fd9d-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1fd9d-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
