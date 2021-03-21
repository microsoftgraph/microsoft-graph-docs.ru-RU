---
title: Get userConsentRequest
description: Ознакомьтесь с свойствами и отношениями объекта userConsentRequest.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8a3a7b1f086462210d77d2ab2f7b61ec116a38c7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965137"
---
# <a name="get-userconsentrequest"></a><span data-ttu-id="aa584-103">Get userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="aa584-103">Get userConsentRequest</span></span>
<span data-ttu-id="aa584-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa584-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa584-105">Ознакомьтесь с свойствами и отношениями [объекта userConsentRequest.](../resources/userconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="aa584-105">Read the properties and relationships of a [userConsentRequest](../resources/userconsentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa584-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa584-106">Permissions</span></span>
<span data-ttu-id="aa584-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa584-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa584-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa584-109">Permission type</span></span>|<span data-ttu-id="aa584-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa584-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa584-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa584-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aa584-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa584-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="aa584-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa584-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa584-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa584-114">Not supported.</span></span>|
|<span data-ttu-id="aa584-115">Application</span><span class="sxs-lookup"><span data-stu-id="aa584-115">Application</span></span>|<span data-ttu-id="aa584-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa584-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa584-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa584-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{appconsentrequest-id}/userConsentRequests/{userconsentrequest-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa584-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aa584-118">Optional query parameters</span></span>
<span data-ttu-id="aa584-119">Этот метод поддерживает параметр  `$select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aa584-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="aa584-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="aa584-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa584-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa584-121">Request headers</span></span>
|<span data-ttu-id="aa584-122">Имя</span><span class="sxs-lookup"><span data-stu-id="aa584-122">Name</span></span>|<span data-ttu-id="aa584-123">Описание</span><span class="sxs-lookup"><span data-stu-id="aa584-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="aa584-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa584-124">Authorization</span></span>|<span data-ttu-id="aa584-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa584-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa584-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa584-127">Request body</span></span>
<span data-ttu-id="aa584-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa584-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa584-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa584-129">Response</span></span>

<span data-ttu-id="aa584-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект userConsentRequest](../resources/userconsentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="aa584-130">If successful, this method returns a `200 OK` response code and a [userConsentRequest](../resources/userconsentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aa584-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="aa584-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aa584-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa584-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_userconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests/acef2660-d194-4943-b927-4fe4fb5cb7e3
```


### <a name="response"></a><span data-ttu-id="aa584-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa584-133">Response</span></span>
<span data-ttu-id="aa584-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="aa584-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests/$entity",
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
```
