---
title: Get appConsentRequest
description: Ознакомьтесь с свойствами и отношениями объекта appConsentRequest.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 766bf7cd58630a74d8f0ac2d0c0982ca87b1d4f0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952241"
---
# <a name="get-appconsentrequest"></a><span data-ttu-id="57d11-103">Get appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="57d11-103">Get appConsentRequest</span></span>
<span data-ttu-id="57d11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57d11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57d11-105">Ознакомьтесь с свойствами и отношениями [объекта appConsentRequest.](../resources/appconsentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="57d11-105">Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="57d11-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57d11-106">Permissions</span></span>
<span data-ttu-id="57d11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57d11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57d11-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57d11-109">Permission type</span></span>|<span data-ttu-id="57d11-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57d11-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57d11-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57d11-111">Delegated (work or school account)</span></span>|<span data-ttu-id="57d11-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57d11-112">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|
|<span data-ttu-id="57d11-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57d11-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57d11-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57d11-114">Not supported.</span></span>|
|<span data-ttu-id="57d11-115">Application</span><span class="sxs-lookup"><span data-stu-id="57d11-115">Application</span></span>|<span data-ttu-id="57d11-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57d11-116">ConsentRequest.Read.All, ConsentRequest.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57d11-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57d11-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/appConsent/appConsentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57d11-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="57d11-118">Optional query parameters</span></span>
<span data-ttu-id="57d11-119">Этот метод поддерживает параметр  `$select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="57d11-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="57d11-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="57d11-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="57d11-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57d11-121">Request headers</span></span>
|<span data-ttu-id="57d11-122">Имя</span><span class="sxs-lookup"><span data-stu-id="57d11-122">Name</span></span>|<span data-ttu-id="57d11-123">Описание</span><span class="sxs-lookup"><span data-stu-id="57d11-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="57d11-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57d11-124">Authorization</span></span>|<span data-ttu-id="57d11-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57d11-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57d11-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57d11-127">Request body</span></span>
<span data-ttu-id="57d11-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57d11-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57d11-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="57d11-129">Response</span></span>

<span data-ttu-id="57d11-130">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект appConsentRequest](../resources/appconsentrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="57d11-130">If successful, this method returns a `200 OK` response code and an [appConsentRequest](../resources/appconsentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57d11-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="57d11-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="57d11-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="57d11-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appconsentrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/appConsent/appConsentRequests/af330b30-dd59-4482-a848-0fd81b0438ed
```


### <a name="response"></a><span data-ttu-id="57d11-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="57d11-133">Response</span></span>
<span data-ttu-id="57d11-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="57d11-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appConsentRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests/$entity",
  "id": "af330b30-dd59-4482-a848-0fd81b0438ed",
  "appId": "3ca5f23f-94b4-4930-aec9-b8ca0f060e68",
  "appDisplayName": "Moodle",
  "consentType": "Dynamic",
  "pendingScopes": [],
  "userConsentRequests@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/appConsent/appConsentRequests('af330b30-dd59-4482-a848-0fd81b0438ed')/userConsentRequests",
  "userConsentRequests": []
}
```

