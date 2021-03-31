---
title: Список appConsentRequests
description: Извлечение объектов appConsentRequest и их свойств
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: fba86e4f48a74097cf278fd20c65769f92b959c4
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469627"
---
# <a name="list-appconsentrequests"></a><span data-ttu-id="7bc03-103">Список appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="7bc03-103">List appConsentRequests</span></span>
<span data-ttu-id="7bc03-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bc03-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7bc03-105">[Извлечение объектов appConsentRequest](../resources/appconsentrequest.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="7bc03-105">Retrieve [appConsentRequest](../resources/appconsentrequest.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="7bc03-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7bc03-106">Permissions</span></span>

<span data-ttu-id="7bc03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bc03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bc03-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bc03-109">Permission type</span></span>|<span data-ttu-id="7bc03-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bc03-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bc03-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bc03-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7bc03-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bc03-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="7bc03-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bc03-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bc03-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bc03-114">Not supported.</span></span>|
|<span data-ttu-id="7bc03-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bc03-115">Application</span></span>|<span data-ttu-id="7bc03-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="7bc03-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bc03-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bc03-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7bc03-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7bc03-118">Optional query parameters</span></span>

<span data-ttu-id="7bc03-119">Этот метод поддерживает  `$select` параметры `$skip` запроса , `$top` , , и `$filter` `$orderby` OData, чтобы помочь настроить ответ.</span><span class="sxs-lookup"><span data-stu-id="7bc03-119">This method supports the `$select`, `$skip`, `$top`, `$filter`, and `$orderby` OData query parameters to help customize the response.</span></span> <span data-ttu-id="7bc03-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7bc03-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7bc03-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bc03-121">Request headers</span></span>

|<span data-ttu-id="7bc03-122">Имя</span><span class="sxs-lookup"><span data-stu-id="7bc03-122">Name</span></span>|<span data-ttu-id="7bc03-123">Описание</span><span class="sxs-lookup"><span data-stu-id="7bc03-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7bc03-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bc03-124">Authorization</span></span>|<span data-ttu-id="7bc03-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bc03-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bc03-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7bc03-127">Request body</span></span>

<span data-ttu-id="7bc03-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7bc03-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bc03-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bc03-129">Response</span></span>

<span data-ttu-id="7bc03-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [appConsentRequest](../resources/appconsentrequest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7bc03-130">If successful, this method returns a `200 OK` response code and a collection of [appConsentRequest](../resources/appconsentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7bc03-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="7bc03-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7bc03-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bc03-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_appconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/appConsent/appConsentRequests
```

### <a name="response"></a><span data-ttu-id="7bc03-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bc03-133">Response</span></span>

<span data-ttu-id="7bc03-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7bc03-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/appConsent/appConsentRequests",
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
