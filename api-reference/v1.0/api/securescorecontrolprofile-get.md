---
title: Получение объектов secureScoreControlProfile
description: Получение свойств и связей объекта Секурескореконтролпрофиле.
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 5a596f51aa64a935fefcfcf85f725d3235f12238
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448297"
---
# <a name="get-securescorecontrolprofile"></a><span data-ttu-id="1a59b-103">Получение объектов secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="1a59b-103">Get secureScoreControlProfile</span></span>

<span data-ttu-id="1a59b-104">Получение свойств и связей объекта [секурескореконтролпрофиле](../resources/securescorecontrolprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="1a59b-104">Retrieve the properties and relationships of an [securescorecontrolprofile](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a59b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a59b-105">Permissions</span></span>

<span data-ttu-id="1a59b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a59b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a59b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a59b-108">Permission type</span></span>      | <span data-ttu-id="1a59b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a59b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a59b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a59b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="1a59b-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a59b-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="1a59b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a59b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1a59b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a59b-113">Not supported.</span></span>  |
|<span data-ttu-id="1a59b-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="1a59b-114">Application</span></span> | <span data-ttu-id="1a59b-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a59b-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a59b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a59b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securescorecontrolprofiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1a59b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a59b-117">Request headers</span></span>

| <span data-ttu-id="1a59b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="1a59b-118">Name</span></span>      |<span data-ttu-id="1a59b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="1a59b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1a59b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a59b-120">Authorization</span></span>  | <span data-ttu-id="1a59b-121">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="1a59b-121">Bearer {code}.</span></span> <span data-ttu-id="1a59b-122">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="1a59b-122">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a59b-123">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="1a59b-123">Request body</span></span>

<span data-ttu-id="1a59b-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1a59b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a59b-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a59b-125">Response</span></span>

<span data-ttu-id="1a59b-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **секурескореконтролпрофиле** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a59b-126">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfile** object in the response body.</span></span> <span data-ttu-id="1a59b-127">Если от поставщика возвращается код состояния, отличный от 2xx или 404, или истекло время ожидания поставщика, откликом будет код состояния `206 Partial Content` с ответом поставщика в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="1a59b-127">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="1a59b-128">Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="1a59b-128">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="1a59b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1a59b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a59b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a59b-130">Request</span></span>

<span data-ttu-id="1a59b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a59b-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1a59b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a59b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofile"
}-->

```http
GET https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1a59b-133">C#</span><span class="sxs-lookup"><span data-stu-id="1a59b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescorecontrolprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1a59b-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="1a59b-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescorecontrolprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1a59b-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1a59b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescorecontrolprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1a59b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a59b-136">Response</span></span>

<span data-ttu-id="1a59b-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1a59b-137">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.secureScoreControlProfile"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "DLPEnabled",
  "azureTenantId": "00000001-0001-0001-0001-000000000001c",
  "actionType": "Config",
  "actionUrl": "https://compliance.microsoft.com/#/policies",
  "controlCategory": "Data",
  "title": "Apply Data Loss Prevention policies", 
  "deprecated": false,
  "implementationCost": "Moderate",
  "lastModifiedDateTime": null,
  "maxScore": 20.0,
  "rank": 55,
  "remediation": "You can create and manage data loss prevention policies in the Policies page of the compliance portal.",
  "remediationImpact": "This change will have a moderate impact on your users.",
  "service": "IP",
  "threats": [
    "Data Exfiltration",
    "Data Spillage"
  ],
  "tier": "Advanced",
  "userImpact": "Moderate",
  "complianceInformation": [
    {
      "certificationName": "ISO 27001:2013",
      "certificationControls": [
        {
          "name": "A.8.2.1",
          "url": "",
        }
      ]
    }         
  ],
  "controlStateUpdates": [
    {
      "assignedTo": null,
      "comment": null,
      "state": "Default",
      "updatedBy": null,
      "updatedDateTime": "2019-03-19T22:37:14.628799Z"
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
  "description": "get secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
