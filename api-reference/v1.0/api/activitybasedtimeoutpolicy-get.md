---
title: Get activityBasedTimeoutPolicy
description: Получите свойства объекта activityBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0830ef84ca3082d5e47deeca9575fd4055d8c358
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442623"
---
# <a name="get-activitybasedtimeoutpolicy"></a><span data-ttu-id="6aa25-103">Get activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="6aa25-103">Get activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="6aa25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6aa25-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="6aa25-105">Получите свойства объекта [activityBasedTimeoutPolicy.](../resources/activitybasedtimeoutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6aa25-105">Get the properties of an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6aa25-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6aa25-106">Permissions</span></span>

<span data-ttu-id="6aa25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6aa25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6aa25-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6aa25-109">Permission type</span></span>                        | <span data-ttu-id="6aa25-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6aa25-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6aa25-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6aa25-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6aa25-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6aa25-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="6aa25-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6aa25-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6aa25-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6aa25-114">Not supported.</span></span> |
| <span data-ttu-id="6aa25-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6aa25-115">Application</span></span>                            | <span data-ttu-id="6aa25-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6aa25-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="6aa25-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6aa25-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6aa25-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6aa25-118">Optional query parameters</span></span>

<span data-ttu-id="6aa25-119">Этот метод поддерживает `$select` параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6aa25-119">This method supports the `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="6aa25-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6aa25-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6aa25-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6aa25-121">Request headers</span></span>

| <span data-ttu-id="6aa25-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6aa25-122">Name</span></span>      |<span data-ttu-id="6aa25-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6aa25-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6aa25-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6aa25-124">Authorization</span></span> | <span data-ttu-id="6aa25-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6aa25-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6aa25-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6aa25-127">Request body</span></span>

<span data-ttu-id="6aa25-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6aa25-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6aa25-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6aa25-129">Response</span></span>

<span data-ttu-id="6aa25-130">В случае успешной работы этот метод возвращает код отклика и запрашиваемого объекта `200 OK` [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6aa25-130">If successful, this method returns a `200 OK` response code and the requested [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6aa25-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="6aa25-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6aa25-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6aa25-132">Request</span></span>

<span data-ttu-id="6aa25-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6aa25-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6aa25-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6aa25-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="6aa25-135">C#</span><span class="sxs-lookup"><span data-stu-id="6aa25-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6aa25-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6aa25-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6aa25-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6aa25-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6aa25-138">Java</span><span class="sxs-lookup"><span data-stu-id="6aa25-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitybasedtimeoutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6aa25-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="6aa25-139">Response</span></span>

<span data-ttu-id="6aa25-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6aa25-140">The following is an example of the response.</span></span>

> <span data-ttu-id="6aa25-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6aa25-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

