---
title: Получение Идентитисекуритидефаултсенфорцементполици
description: Получение свойств и связей объекта идентитисекуритидефаултсенфорцементполици.
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ce5eb0ab5232540127762bbbc94002273eae0416
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001584"
---
# <a name="get-identitysecuritydefaultsenforcementpolicy"></a><span data-ttu-id="e4d3f-103">Получение Идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="e4d3f-103">Get identitySecurityDefaultsEnforcementPolicy</span></span>

<span data-ttu-id="e4d3f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4d3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4d3f-105">Получение свойств объекта [идентитисекуритидефаултсенфорцементполици](../resources/identitysecuritydefaultsenforcementpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="e4d3f-105">Retrieve the properties of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4d3f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4d3f-106">Permissions</span></span>

<span data-ttu-id="e4d3f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4d3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e4d3f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4d3f-109">Permission type</span></span>                        | <span data-ttu-id="e4d3f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4d3f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e4d3f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4d3f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e4d3f-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4d3f-112">Policy.Read.All</span></span> |
| <span data-ttu-id="e4d3f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4d3f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4d3f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4d3f-114">Not supported.</span></span> |
| <span data-ttu-id="e4d3f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4d3f-115">Application</span></span>                            | <span data-ttu-id="e4d3f-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4d3f-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4d3f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4d3f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4d3f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e4d3f-118">Optional query parameters</span></span>

<span data-ttu-id="e4d3f-119">Этот метод поддерживает `select` параметр запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e4d3f-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="e4d3f-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e4d3f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4d3f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4d3f-121">Request headers</span></span>

| <span data-ttu-id="e4d3f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e4d3f-122">Name</span></span>      |<span data-ttu-id="e4d3f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e4d3f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e4d3f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4d3f-124">Authorization</span></span> | <span data-ttu-id="e4d3f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4d3f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4d3f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4d3f-127">Request body</span></span>

<span data-ttu-id="e4d3f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4d3f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4d3f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4d3f-129">Response</span></span>

<span data-ttu-id="e4d3f-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [идентитисекуритидефаултсенфорцементполици](../resources/identitysecuritydefaultsenforcementpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4d3f-130">If successful, this method returns a `200 OK` response code and the requested [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e4d3f-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="e4d3f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e4d3f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4d3f-132">Request</span></span>

<span data-ttu-id="e4d3f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4d3f-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e4d3f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4d3f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identitysecuritydefaultsenforcementpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/identitySecurityDefaultsEnforcementPolicy
```
# <a name="c"></a>[<span data-ttu-id="e4d3f-135">C#</span><span class="sxs-lookup"><span data-stu-id="e4d3f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identitysecuritydefaultsenforcementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4d3f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4d3f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identitysecuritydefaultsenforcementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4d3f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4d3f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identitysecuritydefaultsenforcementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e4d3f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4d3f-138">Response</span></span>

<span data-ttu-id="e4d3f-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e4d3f-139">The following is an example of the response.</span></span>

> <span data-ttu-id="e4d3f-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4d3f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#policies/identitySecurityDefaultsEnforcementPolicy",
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


