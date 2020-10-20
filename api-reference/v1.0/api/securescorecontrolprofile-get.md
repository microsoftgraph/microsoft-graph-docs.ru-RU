---
title: Получение объектов secureScoreControlProfile
description: Получение свойств и связей объекта Секурескореконтролпрофиле.
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 78fc101ee08aec939ec8eb97240fccb5149a1a66
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48601649"
---
# <a name="get-securescorecontrolprofile"></a><span data-ttu-id="58868-103">Получение объектов secureScoreControlProfile</span><span class="sxs-lookup"><span data-stu-id="58868-103">Get secureScoreControlProfile</span></span>

<span data-ttu-id="58868-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58868-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="58868-105">Получение свойств и связей объекта [секурескореконтролпрофиле](../resources/securescorecontrolprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="58868-105">Retrieve the properties and relationships of an [securescorecontrolprofile](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="58868-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58868-106">Permissions</span></span>

<span data-ttu-id="58868-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58868-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58868-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58868-109">Permission type</span></span>      | <span data-ttu-id="58868-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58868-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58868-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58868-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="58868-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58868-112">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span>   |
|<span data-ttu-id="58868-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58868-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="58868-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58868-114">Not supported.</span></span>  |
|<span data-ttu-id="58868-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="58868-115">Application</span></span> | <span data-ttu-id="58868-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58868-116">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58868-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58868-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securescorecontrolprofiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="58868-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58868-118">Request headers</span></span>

| <span data-ttu-id="58868-119">Имя</span><span class="sxs-lookup"><span data-stu-id="58868-119">Name</span></span>      |<span data-ttu-id="58868-120">Описание</span><span class="sxs-lookup"><span data-stu-id="58868-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="58868-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="58868-121">Authorization</span></span>  | <span data-ttu-id="58868-122">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="58868-122">Bearer {code}.</span></span> <span data-ttu-id="58868-123">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="58868-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="58868-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="58868-124">Request body</span></span>

<span data-ttu-id="58868-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="58868-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58868-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="58868-126">Response</span></span>

<span data-ttu-id="58868-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **секурескореконтролпрофиле** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58868-127">If successful, this method returns a `200 OK` response code and a **secureScoreControlProfile** object in the response body.</span></span> <span data-ttu-id="58868-128">Если от поставщика возвращается код состояния, отличный от 2xx или 404, или истекло время ожидания поставщика, откликом будет код состояния `206 Partial Content` с ответом поставщика в заголовке предупреждения.</span><span class="sxs-lookup"><span data-stu-id="58868-128">If a status code other than 2xx or 404 is returned from a provider or if a provider times out, the response will be a `206 Partial Content` status code with the provider's response in a warning header.</span></span> <span data-ttu-id="58868-129">Дополнительные сведения см. в статье [Ответы с ошибками Microsoft Graph Security API](../resources/security-error-codes.md).</span><span class="sxs-lookup"><span data-stu-id="58868-129">For more information, see [Microsoft Graph Security API error responses](../resources/security-error-codes.md).</span></span>

## <a name="example"></a><span data-ttu-id="58868-130">Пример</span><span class="sxs-lookup"><span data-stu-id="58868-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="58868-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="58868-131">Request</span></span>

<span data-ttu-id="58868-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58868-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="58868-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="58868-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofile"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/{id}
```
# <a name="c"></a>[<span data-ttu-id="58868-134">C#</span><span class="sxs-lookup"><span data-stu-id="58868-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescorecontrolprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58868-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58868-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescorecontrolprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58868-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58868-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescorecontrolprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58868-137">Java</span><span class="sxs-lookup"><span data-stu-id="58868-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescorecontrolprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="58868-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="58868-138">Response</span></span>

<span data-ttu-id="58868-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="58868-139">The following is an example of the response.</span></span>
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

