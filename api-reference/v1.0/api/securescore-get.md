---
title: Получение объектов secureScore
description: Получение свойств и связей объекта Секурескоре.
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 5a644aab1b80ac866ce3b67a372a16405b032835
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320050"
---
# <a name="get-securescore"></a><span data-ttu-id="e8c40-103">Получение объектов secureScore</span><span class="sxs-lookup"><span data-stu-id="e8c40-103">Get secureScore</span></span>

<span data-ttu-id="e8c40-104">Получение свойств и связей объекта [секурескоре](../resources/securescore.md) .</span><span class="sxs-lookup"><span data-stu-id="e8c40-104">Retrieve the properties and relationships of a [secureScore](../resources/securescore.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8c40-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8c40-105">Permissions</span></span>

<span data-ttu-id="e8c40-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8c40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8c40-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8c40-108">Permission type</span></span>      | <span data-ttu-id="e8c40-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8c40-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8c40-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8c40-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e8c40-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8c40-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="e8c40-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8c40-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e8c40-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8c40-113">Not supported.</span></span>  |
|<span data-ttu-id="e8c40-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="e8c40-114">Application</span></span> | <span data-ttu-id="e8c40-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8c40-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8c40-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8c40-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e8c40-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8c40-117">Request headers</span></span>

| <span data-ttu-id="e8c40-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e8c40-118">Name</span></span>      |<span data-ttu-id="e8c40-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e8c40-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8c40-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8c40-120">Authorization</span></span>  | <span data-ttu-id="e8c40-121">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="e8c40-121">Bearer {code}.</span></span> <span data-ttu-id="e8c40-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="e8c40-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8c40-123">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="e8c40-123">Request body</span></span>

<span data-ttu-id="e8c40-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8c40-124">Do not supply a request body for this method.</span></span> <span data-ttu-id="e8c40-125">Текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="e8c40-125">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="e8c40-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8c40-126">Response</span></span>

<span data-ttu-id="e8c40-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **секурескоре** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8c40-127">If successful, this method returns a `200 OK` response code and a **secureScore** object in the response body.</span></span> <span data-ttu-id="e8c40-128">Если от поставщика возвращается код состояния, отличный от 2xx или 404, или истекло время ожидания поставщика, откликом будет код состояния `206 Partial Content` с ответом поставщика в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="e8c40-128">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="e8c40-129">Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="e8c40-129">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="e8c40-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e8c40-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8c40-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8c40-131">Request</span></span>

<span data-ttu-id="e8c40-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8c40-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e8c40-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8c40-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescore"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScores/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e8c40-134">C#</span><span class="sxs-lookup"><span data-stu-id="e8c40-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescore-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8c40-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8c40-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescore-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e8c40-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e8c40-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescore-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e8c40-137">Java</span><span class="sxs-lookup"><span data-stu-id="e8c40-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescore-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8c40-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8c40-138">Response</span></span>

<span data-ttu-id="e8c40-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e8c40-139">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScore"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "00000001-0001-0001-0001-000000000001c_2019-03-19",
  "azureTenantId": "00000001-0001-0001-0001-000000000001c",
  "activeUserCount": 0,
  "createdDateTime": "2019-03-19T15:21:00Z",
  "currentScore": 387.0,
  "enabledServices": [
    "HasExchange",
    "HasSharePoint",
    "HasInTune"
  ],
  "licensedUserCount": 100,
  "maxScore": 697.0,
  "averageComparativeScores": [
    {
      "basis": "AllTenants",
      "averageScore": 37.0
    },
    {
      "basis": "TotalSeats",
      "averageScore": 46.0
    },
    {
      "basis": "IndustryTypes",
      "averageScore": 109.0
    }
  ],
  "controlScores": [
    {
      "controlCategory": "Identity",
      "controlName": "AdminMFA",
      "description": "Requiring multi-factor authentication (MFA) for all Azure Active Directory accounts with privileged roles",
      "score": 35.0
    },
    {
      "controlCategory": "Data",
      "controlName": "DLPEnabled",
      "description": "Data Loss Prevention (DLP) policies can be used to comply with business standards and industry regulations.",
      "score": 20.0
    }
  ],
"vendorInformation": {
  "provider": "SecureScore",
  "providerVersion": null,
  "subProvider": null,
  "vendor": "Microsoft"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "get secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
