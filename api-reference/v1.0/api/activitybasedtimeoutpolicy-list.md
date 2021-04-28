---
title: Список действийBasedTimeoutPolicies
description: Получите список объектов activityBasedTimeoutPolicy.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: fe442b506122ee08897c806054f51c67fe10f105
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050670"
---
# <a name="list-activitybasedtimeoutpolicies"></a><span data-ttu-id="5f4bd-103">Список действийBasedTimeoutPolicies</span><span class="sxs-lookup"><span data-stu-id="5f4bd-103">List activityBasedTimeoutPolicies</span></span>

<span data-ttu-id="5f4bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f4bd-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="5f4bd-105">Получите список объектов [activityBasedTimeoutPolicy.](../resources/activitybasedtimeoutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5f4bd-105">Get a list of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f4bd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5f4bd-106">Permissions</span></span>

<span data-ttu-id="5f4bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f4bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5f4bd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5f4bd-109">Permission type</span></span>                        | <span data-ttu-id="5f4bd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5f4bd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5f4bd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5f4bd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f4bd-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="5f4bd-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="5f4bd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5f4bd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f4bd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f4bd-114">Not supported.</span></span> |
| <span data-ttu-id="5f4bd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5f4bd-115">Application</span></span>                            | <span data-ttu-id="5f4bd-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="5f4bd-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f4bd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5f4bd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/activityBasedTimeoutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f4bd-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5f4bd-118">Optional query parameters</span></span>

<span data-ttu-id="5f4bd-119">Этот метод поддерживает параметры `$filter` `$select` `$top` запроса OData и OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5f4bd-119">This method supports the `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="5f4bd-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5f4bd-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f4bd-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5f4bd-121">Request headers</span></span>

| <span data-ttu-id="5f4bd-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5f4bd-122">Name</span></span>      |<span data-ttu-id="5f4bd-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5f4bd-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5f4bd-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5f4bd-124">Authorization</span></span> | <span data-ttu-id="5f4bd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5f4bd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5f4bd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5f4bd-127">Request body</span></span>

<span data-ttu-id="5f4bd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5f4bd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f4bd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f4bd-129">Response</span></span>

<span data-ttu-id="5f4bd-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5f4bd-130">If successful, this method returns a `200 OK` response code and a collection of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f4bd-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="5f4bd-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f4bd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5f4bd-132">Request</span></span>

<span data-ttu-id="5f4bd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5f4bd-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5f4bd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f4bd-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies
```
# <a name="c"></a>[<span data-ttu-id="5f4bd-135">C#</span><span class="sxs-lookup"><span data-stu-id="5f4bd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f4bd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f4bd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f4bd-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f4bd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f4bd-138">Java</span><span class="sxs-lookup"><span data-stu-id="5f4bd-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitybasedtimeoutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5f4bd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5f4bd-139">Response</span></span>

<span data-ttu-id="5f4bd-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5f4bd-140">The following is an example of the response.</span></span>

> <span data-ttu-id="5f4bd-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5f4bd-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List activityBasedTimeoutPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

