---
title: Список appConsentRequests
description: Извлечение объектов appConsentRequest и их свойств.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bab0a202c835c56aaaee1e37a41b1e70d97d3d34
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952240"
---
# <a name="list-appconsentrequests"></a><span data-ttu-id="6dd2a-103">Список appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="6dd2a-103">List appConsentRequests</span></span>
<span data-ttu-id="6dd2a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dd2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dd2a-105">[Извлечение объектов appConsentRequest](../resources/appconsentrequest.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="6dd2a-105">Retrieve [appConsentRequest](../resources/appconsentrequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dd2a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6dd2a-106">Permissions</span></span>
<span data-ttu-id="6dd2a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dd2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dd2a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dd2a-109">Permission type</span></span>|<span data-ttu-id="6dd2a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dd2a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dd2a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dd2a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6dd2a-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dd2a-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="6dd2a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dd2a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dd2a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dd2a-114">Not supported.</span></span>|
|<span data-ttu-id="6dd2a-115">Application</span><span class="sxs-lookup"><span data-stu-id="6dd2a-115">Application</span></span>|<span data-ttu-id="6dd2a-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="6dd2a-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dd2a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dd2a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6dd2a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6dd2a-118">Optional query parameters</span></span>
<span data-ttu-id="6dd2a-119">Этот метод поддерживает  `$select` параметры `$skip` запроса , `$top` , , и `$filter` `$orderby` OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="6dd2a-119">This method supports the `$select`, `$skip`, `$top`, `$filter`, and `$orderby` OData query parameters to help customize the response.</span></span> <span data-ttu-id="6dd2a-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6dd2a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dd2a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6dd2a-121">Request headers</span></span>
|<span data-ttu-id="6dd2a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6dd2a-122">Name</span></span>|<span data-ttu-id="6dd2a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6dd2a-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6dd2a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6dd2a-124">Authorization</span></span>|<span data-ttu-id="6dd2a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6dd2a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dd2a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6dd2a-127">Request body</span></span>
<span data-ttu-id="6dd2a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6dd2a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dd2a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dd2a-129">Response</span></span>

<span data-ttu-id="6dd2a-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [appConsentRequest](../resources/appconsentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6dd2a-130">If successful, this method returns a `200 OK` response code and a collection of [appConsentRequest](../resources/appconsentrequest.md) objects in the response body.</span></span>

## <a name="example-1-list-all-appconsentrequests"></a><span data-ttu-id="6dd2a-131">Пример 1. Список всех appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="6dd2a-131">Example 1: List all appConsentRequests</span></span>

### <a name="request"></a><span data-ttu-id="6dd2a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dd2a-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_appconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests
```


### <a name="response"></a><span data-ttu-id="6dd2a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dd2a-133">Response</span></span>
<span data-ttu-id="6dd2a-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6dd2a-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests",
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

## <a name="example-2-list-all-appconsentrequests-with-at-least-one-userconsentrequest-whose-status-is-inprogress"></a><span data-ttu-id="6dd2a-135">Пример 2. Список всех appConsentRequests по крайней мере с одним пользователемConsentRequest, состояние которого InProgress</span><span class="sxs-lookup"><span data-stu-id="6dd2a-135">Example 2: List all appConsentRequests with at least one userConsentRequest whose status is InProgress</span></span>

### <a name="request"></a><span data-ttu-id="6dd2a-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dd2a-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_appconsentrequest_userconsentrequest_InProgress"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests?$filter=userConsentRequests/any (u:u/status eq 'InProgress')
```


### <a name="response"></a><span data-ttu-id="6dd2a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dd2a-137">Response</span></span>
<span data-ttu-id="6dd2a-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6dd2a-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests",
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

