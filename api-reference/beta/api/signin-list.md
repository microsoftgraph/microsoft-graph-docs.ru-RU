---
title: Перечисление входов
doc_type: apiPageType
description: Описан метод перечисления ресурсов signIn (объектов) из API Microsoft Graph API (REST), что помогает при аудите действий в каталоге (клиенте) (бета-версия).
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5c8ca894571d843305b11402c27ea5f9f688052c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410047"
---
# <a name="list-signins"></a><span data-ttu-id="51041-103">Перечисление входов</span><span class="sxs-lookup"><span data-stu-id="51041-103">List signIns</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51041-104">Получает входы пользователей Azure AD для клиента.</span><span class="sxs-lookup"><span data-stu-id="51041-104">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="51041-105">Входы интерактивного типа (где имя пользователя и пароль передаются в составе маркера проверки подлинности) и успешные федеративные входы в настоящее время включаются в журналы входов.</span><span class="sxs-lookup"><span data-stu-id="51041-105">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="51041-106">Последние входы возвращаются первыми.</span><span class="sxs-lookup"><span data-stu-id="51041-106">The most recent signIns are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="51041-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51041-107">Permissions</span></span>

<span data-ttu-id="51041-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51041-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51041-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51041-110">Permission type</span></span>      | <span data-ttu-id="51041-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51041-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51041-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51041-112">Delegated (work or school account)</span></span> | <span data-ttu-id="51041-113">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="51041-113">AuditLog.Read.All</span></span> |
|<span data-ttu-id="51041-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51041-114">Delegated (work or school account)</span></span> | <span data-ttu-id="51041-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="51041-115">Directory.Read.All</span></span> |
|<span data-ttu-id="51041-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51041-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51041-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="51041-117">Not supported</span></span>   |
|<span data-ttu-id="51041-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51041-118">Application</span></span> | <span data-ttu-id="51041-119">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="51041-119">AuditLog.Read.All</span></span> | 
|<span data-ttu-id="51041-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51041-120">Application</span></span> | <span data-ttu-id="51041-121">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="51041-121">Directory.Read.All</span></span>  | 


<span data-ttu-id="51041-122">Кроме того, приложения должны быть [правильно зарегистрированы](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="51041-122">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="51041-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51041-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="51041-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="51041-124">Optional query parameters</span></span>
<span data-ttu-id="51041-125">Этот метод поддерживает указанные ниже параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="51041-125">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="51041-126">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="51041-126">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="51041-127">Имя</span><span class="sxs-lookup"><span data-stu-id="51041-127">Name</span></span>     |<span data-ttu-id="51041-128">Описание</span><span class="sxs-lookup"><span data-stu-id="51041-128">Description</span></span>                            |<span data-ttu-id="51041-129">Пример</span><span class="sxs-lookup"><span data-stu-id="51041-129">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="51041-130">$filter</span><span class="sxs-lookup"><span data-stu-id="51041-130">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="51041-131">Фильтрует результаты (строки).</span><span class="sxs-lookup"><span data-stu-id="51041-131">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="51041-132">$top</span><span class="sxs-lookup"><span data-stu-id="51041-132">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="51041-133">Задает размер страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="51041-133">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="51041-134">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="51041-134">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="51041-135">Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц.</span><span class="sxs-lookup"><span data-stu-id="51041-135">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="51041-136">Список атрибутов, поддерживаемых параметром $filter</span><span class="sxs-lookup"><span data-stu-id="51041-136">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="51041-137">Имя атрибута</span><span class="sxs-lookup"><span data-stu-id="51041-137">Attribute Name</span></span> |<span data-ttu-id="51041-138">Поддерживаемые операторы</span><span class="sxs-lookup"><span data-stu-id="51041-138">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="51041-139">id</span><span class="sxs-lookup"><span data-stu-id="51041-139">id</span></span>|<span data-ttu-id="51041-140">eq</span><span class="sxs-lookup"><span data-stu-id="51041-140">eq</span></span>|
|<span data-ttu-id="51041-141">userId</span><span class="sxs-lookup"><span data-stu-id="51041-141">userId</span></span>|<span data-ttu-id="51041-142">eq</span><span class="sxs-lookup"><span data-stu-id="51041-142">eq</span></span>|
|<span data-ttu-id="51041-143">appId</span><span class="sxs-lookup"><span data-stu-id="51041-143">appId</span></span>|<span data-ttu-id="51041-144">eq</span><span class="sxs-lookup"><span data-stu-id="51041-144">eq</span></span>|
|<span data-ttu-id="51041-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51041-145">createdDateTime</span></span>| <span data-ttu-id="51041-146">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="51041-146">eq, le, ge</span></span>|
|<span data-ttu-id="51041-147">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="51041-147">userDisplayName</span></span>| <span data-ttu-id="51041-148">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51041-148">eq, startswith</span></span>|
|<span data-ttu-id="51041-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="51041-149">userPrincipalName</span></span>| <span data-ttu-id="51041-150">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51041-150">eq, startswith</span></span>|
|<span data-ttu-id="51041-151">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="51041-151">appDisplayName</span></span>| <span data-ttu-id="51041-152">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51041-152">eq, startswith</span></span>|
|<span data-ttu-id="51041-153">ipAddress</span><span class="sxs-lookup"><span data-stu-id="51041-153">ipAddress</span></span>| <span data-ttu-id="51041-154">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51041-154">eq, startswith</span></span>|
|<span data-ttu-id="51041-155">location/city</span><span class="sxs-lookup"><span data-stu-id="51041-155">location/city</span></span>| <span data-ttu-id="51041-156">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51041-156">eq, startswith</span></span>|
|<span data-ttu-id="51041-157">location/state</span><span class="sxs-lookup"><span data-stu-id="51041-157">location/state</span></span>| <span data-ttu-id="51041-158">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51041-158">eq, startswith</span></span>|
|<span data-ttu-id="51041-159">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="51041-159">location/countryOrRegion</span></span>| <span data-ttu-id="51041-160">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51041-160">eq, startswith</span></span>|
|<span data-ttu-id="51041-161">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="51041-161">status/errorCode</span></span>|<span data-ttu-id="51041-162">eq</span><span class="sxs-lookup"><span data-stu-id="51041-162">eq</span></span>|
|<span data-ttu-id="51041-163">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="51041-163">initiatedBy/user/id</span></span>|<span data-ttu-id="51041-164">eq</span><span class="sxs-lookup"><span data-stu-id="51041-164">eq</span></span>|
|<span data-ttu-id="51041-165">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="51041-165">initiatedBy/user/displayName</span></span>| <span data-ttu-id="51041-166">eq</span><span class="sxs-lookup"><span data-stu-id="51041-166">eq</span></span>|
|<span data-ttu-id="51041-167">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="51041-167">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="51041-168">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51041-168">eq, startswith</span></span>|
|<span data-ttu-id="51041-169">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="51041-169">clientAppUsed</span></span>| <span data-ttu-id="51041-170">eq</span><span class="sxs-lookup"><span data-stu-id="51041-170">eq</span></span>|
|<span data-ttu-id="51041-171">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="51041-171">conditionalAccessStatus</span></span> | <span data-ttu-id="51041-172">eq</span><span class="sxs-lookup"><span data-stu-id="51041-172">eq</span></span>|
|<span data-ttu-id="51041-173">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="51041-173">deviceDetail/browser</span></span>| <span data-ttu-id="51041-174">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51041-174">eq, startswith</span></span>|
|<span data-ttu-id="51041-175">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="51041-175">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="51041-176">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="51041-176">eq, startswith</span></span>|
|<span data-ttu-id="51041-177">correlationId</span><span class="sxs-lookup"><span data-stu-id="51041-177">correlationId</span></span>| <span data-ttu-id="51041-178">eq</span><span class="sxs-lookup"><span data-stu-id="51041-178">eq</span></span>|
|<span data-ttu-id="51041-179">riskDetail</span><span class="sxs-lookup"><span data-stu-id="51041-179">riskDetail</span></span>| <span data-ttu-id="51041-180">eq</span><span class="sxs-lookup"><span data-stu-id="51041-180">eq</span></span>|
|<span data-ttu-id="51041-181">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="51041-181">riskLevelAggregated</span></span>| <span data-ttu-id="51041-182">eq</span><span class="sxs-lookup"><span data-stu-id="51041-182">eq</span></span>|
|<span data-ttu-id="51041-183">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="51041-183">riskLevelDuringSignIn</span></span>| <span data-ttu-id="51041-184">eq</span><span class="sxs-lookup"><span data-stu-id="51041-184">eq</span></span>|
|<span data-ttu-id="51041-185">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="51041-185">riskEventTypes</span></span>| <span data-ttu-id="51041-186">eq</span><span class="sxs-lookup"><span data-stu-id="51041-186">eq</span></span>|
|<span data-ttu-id="51041-187">riskState</span><span class="sxs-lookup"><span data-stu-id="51041-187">riskState</span></span>| <span data-ttu-id="51041-188">eq</span><span class="sxs-lookup"><span data-stu-id="51041-188">eq</span></span>|
|<span data-ttu-id="51041-189">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="51041-189">originalRequestId</span></span>| <span data-ttu-id="51041-190">eq</span><span class="sxs-lookup"><span data-stu-id="51041-190">eq</span></span>|
|<span data-ttu-id="51041-191">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="51041-191">tokenIssuerName</span></span>| <span data-ttu-id="51041-192">eq</span><span class="sxs-lookup"><span data-stu-id="51041-192">eq</span></span>|
|<span data-ttu-id="51041-193">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="51041-193">tokenIssuerType</span></span>| <span data-ttu-id="51041-194">eq</span><span class="sxs-lookup"><span data-stu-id="51041-194">eq</span></span>|
|<span data-ttu-id="51041-195">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="51041-195">resourceDisplayName</span></span>| <span data-ttu-id="51041-196">eq</span><span class="sxs-lookup"><span data-stu-id="51041-196">eq</span></span>|
|<span data-ttu-id="51041-197">resourceId</span><span class="sxs-lookup"><span data-stu-id="51041-197">resourceId</span></span>| <span data-ttu-id="51041-198">eq</span><span class="sxs-lookup"><span data-stu-id="51041-198">eq</span></span>|


## <a name="response"></a><span data-ttu-id="51041-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="51041-199">Response</span></span>
<span data-ttu-id="51041-200">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51041-200">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="51041-201">Пример</span><span class="sxs-lookup"><span data-stu-id="51041-201">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51041-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="51041-202">Request</span></span>
<span data-ttu-id="51041-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51041-203">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="51041-204">HTTP</span><span class="sxs-lookup"><span data-stu-id="51041-204">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="51041-205">C#</span><span class="sxs-lookup"><span data-stu-id="51041-205">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="51041-206">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51041-206">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="51041-207">Цель — C</span><span class="sxs-lookup"><span data-stu-id="51041-207">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="51041-208">Ответ</span><span class="sxs-lookup"><span data-stu-id="51041-208">Response</span></span>
<span data-ttu-id="51041-209">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="51041-209">Here is an example of the response.</span></span> 

><span data-ttu-id="51041-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51041-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  ]
}-->
