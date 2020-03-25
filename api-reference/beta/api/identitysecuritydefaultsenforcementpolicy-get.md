---
title: Получение Идентитисекуритидефаултсенфорцементполици
description: Получение свойств и связей объекта идентитисекуритидефаултсенфорцементполици.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5ab081d6542d8d2c678ab2f8b176739000b668eb
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947126"
---
# <a name="get-identitysecuritydefaultsenforcementpolicy"></a><span data-ttu-id="dfda0-103">Получение Идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="dfda0-103">Get identitySecurityDefaultsEnforcementPolicy</span></span>

<span data-ttu-id="dfda0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfda0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfda0-105">Получение свойств объекта [идентитисекуритидефаултсенфорцементполици](../resources/identitysecuritydefaultsenforcementpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="dfda0-105">Retrieve the properties of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfda0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfda0-106">Permissions</span></span>

<span data-ttu-id="dfda0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfda0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dfda0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfda0-109">Permission type</span></span>                        | <span data-ttu-id="dfda0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfda0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dfda0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfda0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dfda0-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfda0-112">Policy.Read.All</span></span> |
| <span data-ttu-id="dfda0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfda0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfda0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfda0-114">Not supported.</span></span> |
| <span data-ttu-id="dfda0-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="dfda0-115">Application</span></span>                            | <span data-ttu-id="dfda0-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfda0-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfda0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfda0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dfda0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dfda0-118">Optional query parameters</span></span>

<span data-ttu-id="dfda0-119">Этот метод поддерживает параметр `select` запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dfda0-119">This method supports the `select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="dfda0-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="dfda0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfda0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfda0-121">Request headers</span></span>

| <span data-ttu-id="dfda0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="dfda0-122">Name</span></span>      |<span data-ttu-id="dfda0-123">Описание</span><span class="sxs-lookup"><span data-stu-id="dfda0-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dfda0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfda0-124">Authorization</span></span> | <span data-ttu-id="dfda0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfda0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfda0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dfda0-127">Request body</span></span>

<span data-ttu-id="dfda0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dfda0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfda0-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="dfda0-129">Response</span></span>

<span data-ttu-id="dfda0-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [идентитисекуритидефаултсенфорцементполици](../resources/identitysecuritydefaultsenforcementpolicy.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dfda0-130">If successful, this method returns a `200 OK` response code and the requested [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dfda0-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="dfda0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dfda0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfda0-132">Request</span></span>

<span data-ttu-id="dfda0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfda0-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dfda0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfda0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identitysecuritydefaultsenforcementpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/identitySecurityDefaultsEnforcementPolicy
```
# <a name="c"></a>[<span data-ttu-id="dfda0-135">C#</span><span class="sxs-lookup"><span data-stu-id="dfda0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identitysecuritydefaultsenforcementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfda0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfda0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identitysecuritydefaultsenforcementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfda0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfda0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identitysecuritydefaultsenforcementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dfda0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfda0-138">Response</span></span>

<span data-ttu-id="dfda0-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dfda0-139">The following is an example of the response.</span></span>

> <span data-ttu-id="dfda0-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfda0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
