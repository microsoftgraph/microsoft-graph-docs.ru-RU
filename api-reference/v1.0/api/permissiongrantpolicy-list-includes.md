---
title: Список включает коллекцию разрешенийGrantPolicy
description: Извлечение списка наборов условий, в которых описываются условия, при которых событие предоставления разрешений включено в политику предоставления разрешений.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: bc52114f7069b3d9371a19cac1d94ab2c4c3ac99
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051293"
---
# <a name="list-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="b7564-103">Список включает коллекцию разрешенийGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="b7564-103">List includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="b7564-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7564-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b7564-105">Извлечение наборов условий, *включенных* в [permissionGrantPolicy.](../resources/permissiongrantpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b7564-105">Retrieve the condition sets which are *included* in a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b7564-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7564-106">Permissions</span></span>

<span data-ttu-id="b7564-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7564-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7564-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7564-109">Permission type</span></span>      | <span data-ttu-id="b7564-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7564-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7564-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7564-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b7564-112">Policy.Read.PermissionGrant, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7564-112">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |
|<span data-ttu-id="b7564-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7564-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7564-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7564-114">Not supported.</span></span>    |
|<span data-ttu-id="b7564-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7564-115">Application</span></span> | <span data-ttu-id="b7564-116">Policy.Read.PermissionGrant, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7564-116">Policy.Read.PermissionGrant, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7564-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7564-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /policies/permissionGrantPolicies/{id}/includes
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b7564-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b7564-118">Optional query parameters</span></span>

<span data-ttu-id="b7564-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b7564-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7564-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7564-120">Request headers</span></span>

| <span data-ttu-id="b7564-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b7564-121">Name</span></span>           | <span data-ttu-id="b7564-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b7564-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="b7564-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7564-123">Authorization</span></span>  | <span data-ttu-id="b7564-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7564-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b7564-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7564-126">Request body</span></span>

<span data-ttu-id="b7564-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7564-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7564-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7564-128">Response</span></span>

<span data-ttu-id="b7564-129">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b7564-129">If successful, this method returns a `200 OK` response code and a collection of [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7564-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b7564-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7564-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7564-131">Request</span></span>

<span data-ttu-id="b7564-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7564-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b7564-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7564-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_get_includes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/microsoft-application-admin/includes
```
# <a name="c"></a>[<span data-ttu-id="b7564-134">C#</span><span class="sxs-lookup"><span data-stu-id="b7564-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-get-includes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7564-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7564-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-get-includes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7564-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7564-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-get-includes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b7564-137">Java</span><span class="sxs-lookup"><span data-stu-id="b7564-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-get-includes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b7564-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7564-138">Response</span></span>

<span data-ttu-id="b7564-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b7564-139">The following is an example of the response.</span></span>

> <span data-ttu-id="b7564-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b7564-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "811d2da7-443c-43da-96e7-28d285b234e9",
      "permissionClassification": "all",
      "permissionType": "application",
      "resourceApplication": "any",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    },
    {
      "id": "60461179-740e-4d8b-9e00-1456a338c44b",
      "permissionClassification": "all",
      "permissionType": "delegated",
      "resourceApplication": "any",
      "permissions": [ "all" ],
      "clientApplicationIds": [ "all" ],
      "clientApplicationTenantIds": [ "all" ],
      "clientApplicationPublisherIds": [ "all" ],
      "clientApplicationsFromVerifiedPublisherOnly": false
    }
  ]
}
```
