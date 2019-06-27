---
title: Перечисление входов
description: Описан метод перечисления ресурсов signIn (объектов) из API Microsoft Graph API (REST), что помогает при аудите действий в каталоге (клиенте) (бета-версия).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e352a6ede72ef5e6b2b776e9f177680760bed0de
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271633"
---
# <a name="list-signins"></a><span data-ttu-id="66c18-103">Перечисление входов</span><span class="sxs-lookup"><span data-stu-id="66c18-103">List signIns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66c18-104">Получает входы пользователей Azure AD для клиента.</span><span class="sxs-lookup"><span data-stu-id="66c18-104">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="66c18-105">Входы интерактивного типа (где имя пользователя и пароль передаются в составе маркера проверки подлинности) и успешные федеративные входы в настоящее время включаются в журналы входов.</span><span class="sxs-lookup"><span data-stu-id="66c18-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="66c18-106">Последние входы возвращаются первыми.</span><span class="sxs-lookup"><span data-stu-id="66c18-106">The most recent signIns are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="66c18-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66c18-107">Permissions</span></span>

<span data-ttu-id="66c18-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66c18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66c18-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66c18-110">Permission type</span></span>      | <span data-ttu-id="66c18-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66c18-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66c18-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66c18-112">Delegated (work or school account)</span></span> | <span data-ttu-id="66c18-113">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="66c18-113">AuditLog.Read.All</span></span> |
|<span data-ttu-id="66c18-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66c18-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66c18-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="66c18-115">Not supported</span></span>   |
|<span data-ttu-id="66c18-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66c18-116">Application</span></span> | <span data-ttu-id="66c18-117">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="66c18-117">AuditLog.Read.All</span></span> | 

<span data-ttu-id="66c18-118">Кроме того, приложения должны быть [правильно зарегистрированы](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="66c18-118">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="66c18-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66c18-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="66c18-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="66c18-120">Optional query parameters</span></span>
<span data-ttu-id="66c18-121">Этот метод поддерживает указанные ниже параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="66c18-121">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="66c18-122">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="66c18-122">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="66c18-123">Имя</span><span class="sxs-lookup"><span data-stu-id="66c18-123">Name</span></span>     |<span data-ttu-id="66c18-124">Описание</span><span class="sxs-lookup"><span data-stu-id="66c18-124">Description</span></span>                            |<span data-ttu-id="66c18-125">Пример</span><span class="sxs-lookup"><span data-stu-id="66c18-125">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="66c18-126">$filter</span><span class="sxs-lookup"><span data-stu-id="66c18-126">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="66c18-127">Фильтрует результаты (строки).</span><span class="sxs-lookup"><span data-stu-id="66c18-127">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="66c18-128">$top</span><span class="sxs-lookup"><span data-stu-id="66c18-128">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="66c18-129">Задает размер страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="66c18-129">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="66c18-130">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="66c18-130">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="66c18-131">Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц.</span><span class="sxs-lookup"><span data-stu-id="66c18-131">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="66c18-132">Список атрибутов, поддерживаемых параметром $filter</span><span class="sxs-lookup"><span data-stu-id="66c18-132">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="66c18-133">Имя атрибута</span><span class="sxs-lookup"><span data-stu-id="66c18-133">Attribute Name</span></span> |<span data-ttu-id="66c18-134">Поддерживаемые операторы</span><span class="sxs-lookup"><span data-stu-id="66c18-134">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="66c18-135">id</span><span class="sxs-lookup"><span data-stu-id="66c18-135">id</span></span>|<span data-ttu-id="66c18-136">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-136">eq</span></span>|
|<span data-ttu-id="66c18-137">userId</span><span class="sxs-lookup"><span data-stu-id="66c18-137">userId</span></span>|<span data-ttu-id="66c18-138">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-138">eq</span></span>|
|<span data-ttu-id="66c18-139">appId</span><span class="sxs-lookup"><span data-stu-id="66c18-139">appId</span></span>|<span data-ttu-id="66c18-140">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-140">eq</span></span>|
|<span data-ttu-id="66c18-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66c18-141">createdDateTime</span></span>| <span data-ttu-id="66c18-142">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="66c18-142">eq, le, ge</span></span>|
|<span data-ttu-id="66c18-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="66c18-143">userDisplayName</span></span>| <span data-ttu-id="66c18-144">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="66c18-144">eq, startswith</span></span>|
|<span data-ttu-id="66c18-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="66c18-145">userPrincipalName</span></span>| <span data-ttu-id="66c18-146">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="66c18-146">eq, startswith</span></span>|
|<span data-ttu-id="66c18-147">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="66c18-147">appDisplayName</span></span>| <span data-ttu-id="66c18-148">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="66c18-148">eq, startswith</span></span>|
|<span data-ttu-id="66c18-149">ipAddress</span><span class="sxs-lookup"><span data-stu-id="66c18-149">ipAddress</span></span>| <span data-ttu-id="66c18-150">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="66c18-150">eq, startswith</span></span>|
|<span data-ttu-id="66c18-151">location/city</span><span class="sxs-lookup"><span data-stu-id="66c18-151">location/city</span></span>| <span data-ttu-id="66c18-152">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="66c18-152">eq, startswith</span></span>|
|<span data-ttu-id="66c18-153">location/state</span><span class="sxs-lookup"><span data-stu-id="66c18-153">location/state</span></span>| <span data-ttu-id="66c18-154">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="66c18-154">eq, startswith</span></span>|
|<span data-ttu-id="66c18-155">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="66c18-155">location/countryOrRegion</span></span>| <span data-ttu-id="66c18-156">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="66c18-156">eq, startswith</span></span>|
|<span data-ttu-id="66c18-157">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="66c18-157">status/errorCode</span></span>|<span data-ttu-id="66c18-158">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-158">eq</span></span>|
|<span data-ttu-id="66c18-159">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="66c18-159">initiatedBy/user/id</span></span>|<span data-ttu-id="66c18-160">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-160">eq</span></span>|
|<span data-ttu-id="66c18-161">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="66c18-161">initiatedBy/user/displayName</span></span>| <span data-ttu-id="66c18-162">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-162">eq</span></span>|
|<span data-ttu-id="66c18-163">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="66c18-163">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="66c18-164">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="66c18-164">eq, startswith</span></span>|
|<span data-ttu-id="66c18-165">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="66c18-165">clientAppUsed</span></span>| <span data-ttu-id="66c18-166">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-166">eq</span></span>|
|<span data-ttu-id="66c18-167">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="66c18-167">conditionalAccessStatus</span></span> | <span data-ttu-id="66c18-168">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-168">eq</span></span>|
|<span data-ttu-id="66c18-169">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="66c18-169">deviceDetail/browser</span></span>| <span data-ttu-id="66c18-170">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="66c18-170">eq, startswith</span></span>|
|<span data-ttu-id="66c18-171">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="66c18-171">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="66c18-172">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="66c18-172">eq, startswith</span></span>|
|<span data-ttu-id="66c18-173">correlationId</span><span class="sxs-lookup"><span data-stu-id="66c18-173">correlationId</span></span>| <span data-ttu-id="66c18-174">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-174">eq</span></span>|
|<span data-ttu-id="66c18-175">riskDetail</span><span class="sxs-lookup"><span data-stu-id="66c18-175">riskDetail</span></span>| <span data-ttu-id="66c18-176">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-176">eq</span></span>|
|<span data-ttu-id="66c18-177">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="66c18-177">riskLevelAggregated</span></span>| <span data-ttu-id="66c18-178">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-178">eq</span></span>|
|<span data-ttu-id="66c18-179">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="66c18-179">riskLevelDuringSignIn</span></span>| <span data-ttu-id="66c18-180">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-180">eq</span></span>|
|<span data-ttu-id="66c18-181">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="66c18-181">riskEventTypes</span></span>| <span data-ttu-id="66c18-182">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-182">eq</span></span>|
|<span data-ttu-id="66c18-183">riskState</span><span class="sxs-lookup"><span data-stu-id="66c18-183">riskState</span></span>| <span data-ttu-id="66c18-184">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-184">eq</span></span>|
|<span data-ttu-id="66c18-185">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="66c18-185">originalRequestId</span></span>| <span data-ttu-id="66c18-186">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-186">eq</span></span>|
|<span data-ttu-id="66c18-187">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="66c18-187">tokenIssuerName</span></span>| <span data-ttu-id="66c18-188">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-188">eq</span></span>|
|<span data-ttu-id="66c18-189">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="66c18-189">tokenIssuerType</span></span>| <span data-ttu-id="66c18-190">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-190">eq</span></span>|
|<span data-ttu-id="66c18-191">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="66c18-191">resourceDisplayName</span></span>| <span data-ttu-id="66c18-192">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-192">eq</span></span>|
|<span data-ttu-id="66c18-193">resourceId</span><span class="sxs-lookup"><span data-stu-id="66c18-193">resourceId</span></span>| <span data-ttu-id="66c18-194">eq</span><span class="sxs-lookup"><span data-stu-id="66c18-194">eq</span></span>|


## <a name="response"></a><span data-ttu-id="66c18-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="66c18-195">Response</span></span>
<span data-ttu-id="66c18-196">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66c18-196">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="66c18-197">Пример</span><span class="sxs-lookup"><span data-stu-id="66c18-197">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66c18-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="66c18-198">Request</span></span>
<span data-ttu-id="66c18-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66c18-199">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a><span data-ttu-id="66c18-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="66c18-200">Response</span></span>
<span data-ttu-id="66c18-201">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="66c18-201">Here is an example of the response.</span></span> 

><span data-ttu-id="66c18-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66c18-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 264
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="66c18-204">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="66c18-204">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="66c18-205">C#</span><span class="sxs-lookup"><span data-stu-id="66c18-205">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_signins-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66c18-206">Javascript</span><span class="sxs-lookup"><span data-stu-id="66c18-206">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_signins-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="66c18-207">Цель — C</span><span class="sxs-lookup"><span data-stu-id="66c18-207">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_signins-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
```json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "value": [{
        "id":"b01b1726-0147-425e-a7f7-21f252050400",
        "createdDateTime":"2018-11-06T18:48:33.8527147Z",
        "userDisplayName":"Jon Doe",
         "userPrincipalName":"admin@aad171.ccsctp.net",
         "userId":"d7cc485d-2c1b-422c-98fd-5ce52859a4a3",
        "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
         "appDisplayName":"Azure Portal",
         "ipAddress":"207.254.19.10",
         "clientAppUsed":"Browser",
        "mfaDetail":null,
         "correlationId":"65dd87ce-2183-419e-81a9-d6e20379bcc2",
         "conditionalAccessStatus":"notApplied",
        "originalRequestId":null,
        "isInteractive":true,
        "tokenIssuerName":null,
        "tokenIssuerType":"AzureAD",
        "processingTimeInMilliseconds":0,
        "riskDetail":"none",
        "riskLevelAggregated":"none",
        "riskLevelDuringSignIn":"none",
        "riskState":"none",
        "riskEventTypes":[

        ],
        "resourceDisplayName":"windows azure service management api",
        "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
        "authenticationMethodsUsed":[

        ],
        "status":{
            "errorCode":50140,
            "failureReason":"This error occurred due to 'Keep me signed in' interrupt when the user was signing-in.",
            "additionalDetails":null
        },
        "deviceDetail":{
            "deviceId":null,
            "displayName":null,
            "operatingSystem":"Windows 7",
            "browser":"Chrome 63.0.3239",
            "isCompliant":null,
            "isManaged":null,
            "trustType":null
        },
        "location":{
            "city":"Lithia Springs",
            "state":"Georgia",
            "countryOrRegion":"US",
            "geoCoordinates":{
                "altitude":null,
                "latitude":33.7930908203125,
                "longitude":-84.445358276367188
            }
        },
        "appliedConditionalAccessPolicies":[
            {
            "id":"6551c58c-e5da-4036-a6ea-c2c3fad264f1",
            "displayName":"New Name here4",
            "enforcedGrantControls":[
                "Mfa",
                "RequireCompliantDevice"
            ],
            "enforcedSessionControls":[

            ],
            "result":"notApplied"
            },
            {
            "id":"b645a140-20fe-4ce0-a724-18ab201e9026",
            "displayName":"PipelineTest4",
            "enforcedGrantControls":[

            ],
            "enforcedSessionControls":[

            ],
            "result":"notEnabled"
            }
        ],
        "authenticationProcessingDetails":[

        ],
        "networkLocationDetails":[

        ]
        }
    
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List signIns",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
