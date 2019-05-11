---
title: Получение объектов secureScore
description: Получение свойств и связей объекта Секурескоре.
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 22bdce327d8f14bf338efc4f5bad709819a6421c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951326"
---
# <a name="get-securescore"></a><span data-ttu-id="c6ea1-103">Получение объектов secureScore</span><span class="sxs-lookup"><span data-stu-id="c6ea1-103">Get secureScore</span></span>

<span data-ttu-id="c6ea1-104">Получение свойств и связей объекта [секурескоре](../resources/securescore.md) .</span><span class="sxs-lookup"><span data-stu-id="c6ea1-104">Retrieve the properties and relationships of a [secureScore](../resources/securescore.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6ea1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6ea1-105">Permissions</span></span>

<span data-ttu-id="c6ea1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6ea1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6ea1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6ea1-108">Permission type</span></span>      | <span data-ttu-id="c6ea1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6ea1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6ea1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6ea1-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c6ea1-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6ea1-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="c6ea1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6ea1-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c6ea1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6ea1-113">Not supported.</span></span>  |
|<span data-ttu-id="c6ea1-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="c6ea1-114">Application</span></span> | <span data-ttu-id="c6ea1-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6ea1-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6ea1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6ea1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScores/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c6ea1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6ea1-117">Request headers</span></span>

| <span data-ttu-id="c6ea1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c6ea1-118">Name</span></span>      |<span data-ttu-id="c6ea1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c6ea1-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c6ea1-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6ea1-120">Authorization</span></span>  | <span data-ttu-id="c6ea1-121">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="c6ea1-121">Bearer {code}.</span></span> <span data-ttu-id="c6ea1-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c6ea1-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6ea1-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6ea1-123">Request body</span></span>

<span data-ttu-id="c6ea1-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c6ea1-124">Do not supply a request body for this method.</span></span> <span data-ttu-id="c6ea1-125">Текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="c6ea1-125">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="c6ea1-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6ea1-126">Response</span></span>

<span data-ttu-id="c6ea1-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **секурескоре** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c6ea1-127">If successful, this method returns a `200 OK` response code and a **secureScore** object in the response body.</span></span> <span data-ttu-id="c6ea1-128">Если от поставщика возвращается код состояния, отличный от 2xx или 404, или истекло время ожидания поставщика, откликом будет код состояния `206 Partial Content` с ответом поставщика в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="c6ea1-128">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="c6ea1-129">Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="c6ea1-129">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="c6ea1-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c6ea1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6ea1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6ea1-131">Request</span></span>

<span data-ttu-id="c6ea1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6ea1-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securescore"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScores/{id}
```

### <a name="response"></a><span data-ttu-id="c6ea1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6ea1-133">Response</span></span>

<span data-ttu-id="c6ea1-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c6ea1-134">The following is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c6ea1-135">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="c6ea1-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c6ea1-136">C#</span><span class="sxs-lookup"><span data-stu-id="c6ea1-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_securescore-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6ea1-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="c6ea1-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_securescore-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "get secureScores",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/securescore-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/securescore-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
