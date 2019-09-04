---
title: Перечисление объектов secureScoreControlProfiles
description: Получение свойств и связей объекта Секурескореконтролпрофилес.
author: preetikr
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 004cc602bcee9e044c1afb4feccc15d73d44b0ae
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36729275"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="4e2cd-103">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="4e2cd-103">List secureScoreControlProfiles</span></span>

<span data-ttu-id="4e2cd-104">Получение свойств и связей объекта [секурескореконтролпрофилес](../resources/securescorecontrolprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="4e2cd-104">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e2cd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4e2cd-105">Permissions</span></span>

<span data-ttu-id="4e2cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e2cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e2cd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e2cd-108">Permission type</span></span>      | <span data-ttu-id="4e2cd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e2cd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e2cd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e2cd-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4e2cd-111">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="4e2cd-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="4e2cd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e2cd-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4e2cd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e2cd-113">Not supported.</span></span>  |
|<span data-ttu-id="4e2cd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4e2cd-114">Application</span></span> | <span data-ttu-id="4e2cd-115">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="4e2cd-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e2cd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e2cd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
GET /security/secureScoreControlProfiles?$top=1
GET /security/secureScoreControlProfiles?$filter={property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4e2cd-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4e2cd-117">Optional query parameters</span></span>

<span data-ttu-id="4e2cd-118">Этот метод поддерживает указанные ниже [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4e2cd-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="4e2cd-119">`$top` возвращает объединенные лучшие результаты от каждого поставщика API безопасности.</span><span class="sxs-lookup"><span data-stu-id="4e2cd-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="4e2cd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4e2cd-120">Request headers</span></span>

| <span data-ttu-id="4e2cd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4e2cd-121">Name</span></span>      |<span data-ttu-id="4e2cd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4e2cd-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4e2cd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4e2cd-123">Authorization</span></span>  | <span data-ttu-id="4e2cd-124">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="4e2cd-124">Bearer {code}.</span></span> <span data-ttu-id="4e2cd-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4e2cd-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e2cd-126">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="4e2cd-126">Request body</span></span>

<span data-ttu-id="4e2cd-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4e2cd-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="4e2cd-128">Текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="4e2cd-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="4e2cd-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e2cd-129">Response</span></span>

<span data-ttu-id="4e2cd-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов **секурескореконтролпрофилес** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4e2cd-130">If successful, this method returns a `200 OK` response code and collection of **secureScoreControlProfiles** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e2cd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4e2cd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e2cd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e2cd-132">Request</span></span>

<span data-ttu-id="4e2cd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e2cd-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4e2cd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e2cd-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofiles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4e2cd-135">C#</span><span class="sxs-lookup"><span data-stu-id="4e2cd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securescorecontrolprofiles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4e2cd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e2cd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securescorecontrolprofiles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4e2cd-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4e2cd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securescorecontrolprofiles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4e2cd-138">Java</span><span class="sxs-lookup"><span data-stu-id="4e2cd-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securescorecontrolprofiles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4e2cd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e2cd-139">Response</span></span>

<span data-ttu-id="4e2cd-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4e2cd-140">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfile",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
  "value": [
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
              "name":  "A.8.2.1",
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
  ]
}
```


<!--
{
  "type": "#page.annotation",
  "description": "List secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
