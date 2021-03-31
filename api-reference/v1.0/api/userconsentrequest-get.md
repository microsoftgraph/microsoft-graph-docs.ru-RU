---
title: Get userConsentRequest
description: Ознакомьтесь с свойствами и отношениями объекта userConsentRequest.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6ee2823c4312a3e0fc98f307826efe542ef304ec
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469711"
---
# <a name="get-userconsentrequest"></a><span data-ttu-id="77e1d-103">Get userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="77e1d-103">Get userConsentRequest</span></span>

<span data-ttu-id="77e1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77e1d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="77e1d-105">Ознакомьтесь с свойствами и отношениями [объекта userConsentRequest.](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="77e1d-105">Read the properties and relationships of a [userConsentRequest](../resources/userconsentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="77e1d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77e1d-106">Permissions</span></span>

<span data-ttu-id="77e1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77e1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77e1d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77e1d-109">Permission type</span></span>|<span data-ttu-id="77e1d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77e1d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77e1d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77e1d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="77e1d-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77e1d-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="77e1d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77e1d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77e1d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77e1d-114">Not supported.</span></span>|
|<span data-ttu-id="77e1d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77e1d-115">Application</span></span>|<span data-ttu-id="77e1d-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77e1d-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77e1d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77e1d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{appconsentrequest-id}/userConsentRequests/{userconsentrequest-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77e1d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="77e1d-118">Optional query parameters</span></span>

<span data-ttu-id="77e1d-119">Этот метод поддерживает параметр  `$select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="77e1d-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="77e1d-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="77e1d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="77e1d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77e1d-121">Request headers</span></span>

|<span data-ttu-id="77e1d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="77e1d-122">Name</span></span>|<span data-ttu-id="77e1d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="77e1d-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="77e1d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77e1d-124">Authorization</span></span>|<span data-ttu-id="77e1d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77e1d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="77e1d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="77e1d-127">Request body</span></span>

<span data-ttu-id="77e1d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77e1d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77e1d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="77e1d-129">Response</span></span>

<span data-ttu-id="77e1d-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект userConsentRequest](../resources/userconsentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="77e1d-130">If successful, this method returns a `200 OK` response code and a [userConsentRequest](../resources/userconsentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="77e1d-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="77e1d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="77e1d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="77e1d-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_userconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests/acef2660-d194-4943-b927-4fe4fb5cb7e3
```

### <a name="response"></a><span data-ttu-id="77e1d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="77e1d-133">Response</span></span>

<span data-ttu-id="77e1d-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="77e1d-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userConsentRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests",
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
  "approval@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests('acef2660-d194-4943-b927-4fe4fb5cb7e3')/approval/$entity",
  "approval": {
    "id": "acef2660-d194-4943-b927-4fe4fb5cb7e3",
    "stages@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests('acef2660-d194-4943-b927-4fe4fb5cb7e3')/approval/stages",
    "stages": [
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
```
