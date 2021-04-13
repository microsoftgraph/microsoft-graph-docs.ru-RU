---
title: Список userConsentRequests
description: Извлечение объектов userConsentRequest и их свойств.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b2ee1d8027ce5685de094e3b10368295fa8319ad
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/13/2021
ms.locfileid: "51698036"
---
# <a name="list-userconsentrequests"></a><span data-ttu-id="49015-103">Список userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="49015-103">List userConsentRequests</span></span>
<span data-ttu-id="49015-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49015-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49015-105">Извлечение коллекции [объектов userConsentRequest](../resources/userconsentrequest.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="49015-105">Retrieve a collection of [userConsentRequest](../resources/userconsentrequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="49015-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49015-106">Permissions</span></span>
<span data-ttu-id="49015-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49015-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49015-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49015-109">Permission type</span></span>|<span data-ttu-id="49015-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49015-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49015-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49015-111">Delegated (work or school account)</span></span>|<span data-ttu-id="49015-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49015-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="49015-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49015-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49015-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49015-114">Not supported.</span></span>|
|<span data-ttu-id="49015-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49015-115">Application</span></span>|<span data-ttu-id="49015-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49015-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="49015-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49015-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{id}/userConsentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49015-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="49015-118">Optional query parameters</span></span>
<span data-ttu-id="49015-119">Этот метод поддерживает  `$select` параметры `$skip` запроса , `$top` , , и `$filter` `$orderby` OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="49015-119">This method supports the `$select`, `$skip`, `$top`, `$filter`, and `$orderby` OData query parameters to help customize the response.</span></span> <span data-ttu-id="49015-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="49015-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="49015-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49015-121">Request headers</span></span>
|<span data-ttu-id="49015-122">Имя</span><span class="sxs-lookup"><span data-stu-id="49015-122">Name</span></span>|<span data-ttu-id="49015-123">Описание</span><span class="sxs-lookup"><span data-stu-id="49015-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="49015-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="49015-124">Authorization</span></span>|<span data-ttu-id="49015-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49015-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="49015-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49015-127">Request body</span></span>
<span data-ttu-id="49015-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="49015-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49015-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="49015-129">Response</span></span>

<span data-ttu-id="49015-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [userConsentRequest](../resources/userconsentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="49015-130">If successful, this method returns a `200 OK` response code and a collection of [userConsentRequest](../resources/userconsentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49015-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="49015-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="49015-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="49015-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="49015-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="49015-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_userconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/ee245379-e3bb-4944-a997-24115f0b8b5e/userConsentRequests
```
# <a name="c"></a>[<span data-ttu-id="49015-134">C#</span><span class="sxs-lookup"><span data-stu-id="49015-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-userconsentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49015-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49015-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-userconsentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49015-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49015-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-userconsentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49015-137">Java</span><span class="sxs-lookup"><span data-stu-id="49015-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-userconsentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="49015-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="49015-138">Response</span></span>
<span data-ttu-id="49015-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="49015-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('ee245379-e3bb-4944-a997-24115f0b8b5e')/userConsentRequests",
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
