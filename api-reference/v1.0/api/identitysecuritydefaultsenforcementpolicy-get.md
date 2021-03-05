---
title: Get identitySecurityDefaultsEnforcementPolicy
description: Извлечение свойств и связей объекта identitysecuritydefaultsenforcementpolicy.
localization_priority: Normal
author: rohinigoyal1
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 927de49830838e219b164eaac1be4fbcd7d657e9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441832"
---
# <a name="get-identitysecuritydefaultsenforcementpolicy"></a><span data-ttu-id="5d29d-103">Get identitySecurityDefaultsEnforcementPolicy</span><span class="sxs-lookup"><span data-stu-id="5d29d-103">Get identitySecurityDefaultsEnforcementPolicy</span></span>

<span data-ttu-id="5d29d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d29d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d29d-105">Извлечение свойств [объекта identitySecurityDefaultsEnforcementPolicy.](../resources/identitysecuritydefaultsenforcementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="5d29d-105">Retrieve the properties of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d29d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d29d-106">Permissions</span></span>

<span data-ttu-id="5d29d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d29d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5d29d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d29d-109">Permission type</span></span>                        | <span data-ttu-id="5d29d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d29d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5d29d-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d29d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d29d-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d29d-112">Policy.Read.All</span></span> |
| <span data-ttu-id="5d29d-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d29d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d29d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d29d-114">Not supported.</span></span> |
| <span data-ttu-id="5d29d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d29d-115">Application</span></span>                            | <span data-ttu-id="5d29d-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d29d-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d29d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d29d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5d29d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5d29d-118">Optional query parameters</span></span>

<span data-ttu-id="5d29d-119">Этот метод поддерживает параметр `select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5d29d-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="5d29d-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5d29d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d29d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d29d-121">Request headers</span></span>

| <span data-ttu-id="5d29d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5d29d-122">Name</span></span>      |<span data-ttu-id="5d29d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5d29d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5d29d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d29d-124">Authorization</span></span> | <span data-ttu-id="5d29d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d29d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d29d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d29d-127">Request body</span></span>

<span data-ttu-id="5d29d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5d29d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d29d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d29d-129">Response</span></span>

<span data-ttu-id="5d29d-130">В случае успешного выполнения этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5d29d-130">If successful, this method returns a `200 OK` response code and the requested [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5d29d-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="5d29d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5d29d-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d29d-132">Request</span></span>

<span data-ttu-id="5d29d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d29d-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5d29d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d29d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identitysecuritydefaultsenforcementpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/identitySecurityDefaultsEnforcementPolicy
```
# <a name="c"></a>[<span data-ttu-id="5d29d-135">C#</span><span class="sxs-lookup"><span data-stu-id="5d29d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identitysecuritydefaultsenforcementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d29d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d29d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identitysecuritydefaultsenforcementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d29d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d29d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identitysecuritydefaultsenforcementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5d29d-138">Java</span><span class="sxs-lookup"><span data-stu-id="5d29d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identitysecuritydefaultsenforcementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5d29d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d29d-139">Response</span></span>

<span data-ttu-id="5d29d-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5d29d-140">The following is an example of the response.</span></span>

> <span data-ttu-id="5d29d-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d29d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/identitySecurityDefaultsEnforcementPolicy",
  "description": "Security defaults is a set of basic identity security mechanisms recommended by Microsoft. When enabled, these recommendations will be automatically enforced in your organization. Administrators and users will be better protected from common identity related attacks.",
  "displayName": "Security Defaults",
  "id": "00000000-0000-0000-0000-000000000005",
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identitySecurityDefaultsEnforcementPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

