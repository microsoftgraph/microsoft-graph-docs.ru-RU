---
title: Получить permissionGrantPolicy
description: Извлечение одного объекта permissionGrantPolicy.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 7065399613ceb1eaa2c797afadb511a5bf2b62e5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433973"
---
# <a name="get-permissiongrantpolicy"></a><span data-ttu-id="f0180-103">Получить permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="f0180-103">Get permissionGrantPolicy</span></span>

<span data-ttu-id="f0180-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0180-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0180-105">Извлечение одного [объекта permissionGrantPolicy.](../resources/permissiongrantpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f0180-105">Retrieve a single [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0180-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f0180-106">Permissions</span></span>

<span data-ttu-id="f0180-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0180-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f0180-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0180-109">Permission type</span></span>                        | <span data-ttu-id="f0180-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0180-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f0180-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0180-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f0180-112">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f0180-112">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="f0180-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0180-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0180-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0180-114">Not supported.</span></span> |
| <span data-ttu-id="f0180-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f0180-115">Application</span></span>                            | <span data-ttu-id="f0180-116">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="f0180-116">Policy.Read.PermissionGrant, Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0180-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0180-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/permissionGrantPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0180-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f0180-118">Optional query parameters</span></span>

<span data-ttu-id="f0180-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="f0180-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0180-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0180-120">Request headers</span></span>

| <span data-ttu-id="f0180-121">Имя</span><span class="sxs-lookup"><span data-stu-id="f0180-121">Name</span></span>           | <span data-ttu-id="f0180-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f0180-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f0180-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f0180-123">Authorization</span></span>  | <span data-ttu-id="f0180-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0180-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f0180-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f0180-126">Request body</span></span>

<span data-ttu-id="f0180-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0180-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0180-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0180-128">Response</span></span>

<span data-ttu-id="f0180-129">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [permissionGrantPolicy](../resources/permissiongrantpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f0180-129">If successful, this method returns a `200 OK` response code and the requested [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0180-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="f0180-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f0180-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0180-131">Request</span></span>

<span data-ttu-id="f0180-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0180-132">The following is an example of the request.</span></span> <span data-ttu-id="f0180-133">В этом примере запрашиваемой политикой является встроенная политика предоставления разрешений, которая включает делегирование разрешений, классифицированных с низким уровнем, для приложений от проверенных издателей или приложений, зарегистрированных в `microsoft-user-default-low` этом клиенте.</span><span class="sxs-lookup"><span data-stu-id="f0180-133">In this example, the requested policy is the built-in permission grant policy `microsoft-user-default-low`, which includes delegated permissions classified low, for apps from verified publishers or apps registered in this tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="f0180-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0180-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_permissiongrantpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/permissionGrantPolicies/microsoft-user-default-low
```
# <a name="c"></a>[<span data-ttu-id="f0180-135">C#</span><span class="sxs-lookup"><span data-stu-id="f0180-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0180-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0180-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0180-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0180-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0180-138">Java</span><span class="sxs-lookup"><span data-stu-id="f0180-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-permissiongrantpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f0180-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0180-139">Response</span></span>

<span data-ttu-id="f0180-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f0180-140">The following is an example of the response.</span></span> <span data-ttu-id="f0180-141">Политика имеет два набора условий, один из которых совпадает с делегированным разрешением, классифицированным для клиентских приложений, зарегистрированных в этом клиенте, и другой, который соответствует делегированию разрешений, классифицированных для приложений от проверенных издателей (независимо от того, в каком клиенте зарегистрировано `includes` `low` `low` приложение).</span><span class="sxs-lookup"><span data-stu-id="f0180-141">The policy has two `includes` condition sets, one which matches with delegated permission classified `low` for client apps registered in this tenant, and the other which matches delegated permissions classified `low` for apps from verified publishers (regardless of which tenant the app is registered in).</span></span>

> <span data-ttu-id="f0180-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0180-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "microsoft-user-default-low",
    "displayName": "Default User Low Risk Policy",
    "description": "All low risk permissions are consentable by member type users by default.",
    "includes": [
        {
            "id": "cb0c20dd-919d-40c5-ba6d-7ffb233b4b0b",
            "permissionClassification": "low",
            "permissionType": "delegated",
            "resourceApplication": "any",
            "permissions": [ "all" ],
            "clientApplicationIds": [ "all" ],
            "clientApplicationTenantIds": [ "11e37ee2-48fe-42e0-aab9-07d0bb165353" ],
            "clientApplicationPublisherIds": [ "all" ],
            "clientApplicationsFromVerifiedPublisherOnly": false
        },
        {
            "id": "8ce99f96-730c-4ebd-8397-07ee65942b97",
            "permissionClassification": "low",
            "permissionType": "delegated",
            "resourceApplication": "any",
            "permissions": [ "all" ],
            "clientApplicationIds": [ "all" ],
            "clientApplicationTenantIds": [ "all" ],
            "clientApplicationPublisherIds": [ "all" ],
            "clientApplicationsFromVerifiedPublisherOnly": true
        }
    ],
    "excludes": []
}
```
