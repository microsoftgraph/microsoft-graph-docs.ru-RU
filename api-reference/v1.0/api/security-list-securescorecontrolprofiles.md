---
title: Перечисление объектов secureScoreControlProfiles
description: Получение свойств и связей объекта Секурескореконтролпрофилес.
author: preetikr
localization_priority: Normal
ms.openlocfilehash: d7de3b6b446aa12447023d6b4f111fc2ac28b41e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629742"
---
# <a name="list-securescorecontrolprofiles"></a><span data-ttu-id="dd2c2-103">Перечисление объектов secureScoreControlProfiles</span><span class="sxs-lookup"><span data-stu-id="dd2c2-103">List secureScoreControlProfiles</span></span>

<span data-ttu-id="dd2c2-104">Получение свойств и связей объекта [секурескореконтролпрофилес](../resources/securescorecontrolprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="dd2c2-104">Retrieve the properties and relationships of a [secureScoreControlProfiles](../resources/securescorecontrolprofile.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd2c2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd2c2-105">Permissions</span></span>

<span data-ttu-id="dd2c2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd2c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd2c2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd2c2-108">Permission type</span></span>      | <span data-ttu-id="dd2c2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd2c2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd2c2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd2c2-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="dd2c2-111">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="dd2c2-111">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span>   |
|<span data-ttu-id="dd2c2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd2c2-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="dd2c2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd2c2-113">Not supported.</span></span>  |
|<span data-ttu-id="dd2c2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd2c2-114">Application</span></span> | <span data-ttu-id="dd2c2-115">Область securityevents. Read. ALL, область securityevents. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="dd2c2-115">SecurityEvents.Read.All, SecurityEvents.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd2c2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd2c2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/secureScoreControlProfiles
GET /security/secureScoreControlProfiles?$top=1
GET /security/secureScoreControlProfiles?$filter={property} eq '{property-value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd2c2-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dd2c2-117">Optional query parameters</span></span>

<span data-ttu-id="dd2c2-118">Этот метод поддерживает указанные ниже [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="dd2c2-118">This method supports the following [OData query parameters](/graph/query-parameters) to help customize the response:</span></span>

- `$count`
- `$filter`
- `$skip`
- <span data-ttu-id="dd2c2-119">`$top` возвращает объединенные лучшие результаты от каждого поставщика API безопасности.</span><span class="sxs-lookup"><span data-stu-id="dd2c2-119">`$top` will return the aggregated top results from each security API provider.</span></span>  

## <a name="request-headers"></a><span data-ttu-id="dd2c2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd2c2-120">Request headers</span></span>

| <span data-ttu-id="dd2c2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="dd2c2-121">Name</span></span>      |<span data-ttu-id="dd2c2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dd2c2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dd2c2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd2c2-123">Authorization</span></span>  | <span data-ttu-id="dd2c2-124">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="dd2c2-124">Bearer {code}.</span></span> <span data-ttu-id="dd2c2-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="dd2c2-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd2c2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd2c2-126">Request body</span></span>

<span data-ttu-id="dd2c2-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd2c2-127">Do not supply a request body for this method.</span></span> <span data-ttu-id="dd2c2-128">Текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="dd2c2-128">The request body will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="dd2c2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd2c2-129">Response</span></span>

<span data-ttu-id="dd2c2-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов **секурескореконтролпрофилес** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd2c2-130">If successful, this method returns a `200 OK` response code and collection of **secureScoreControlProfiles** objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd2c2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="dd2c2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd2c2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd2c2-132">Request</span></span>

<span data-ttu-id="dd2c2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd2c2-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_securescorecontrolprofiles"
}-->

```http
GET https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles
```

### <a name="response"></a><span data-ttu-id="dd2c2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd2c2-134">Response</span></span>

<span data-ttu-id="dd2c2-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dd2c2-135">The following is an example of the response.</span></span>
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
  "tocPath": ""
}
-->
