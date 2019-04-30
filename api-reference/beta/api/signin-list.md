---
title: Перечисление входов
description: Извлекает входы пользователей Azure AD для клиента. Входы интерактивного типа (где имя пользователя и пароль передаются в составе маркера проверки подлинности) и успешные федеративные входы в настоящее время включаются в журналы входов.  Последние входы возвращаются первыми.
localization_priority: Priority
ms.openlocfilehash: 8596bd168a3e10cbea9e15e2f61d6bd668fd27b5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545159"
---
# <a name="list-signins"></a><span data-ttu-id="b7649-105">Перечисление входов</span><span class="sxs-lookup"><span data-stu-id="b7649-105">List sign-ins</span></span>

<span data-ttu-id="b7649-106">Извлекает входы пользователей Azure AD для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7649-106">Retrieves the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="b7649-107">Входы интерактивного типа (где имя пользователя и пароль передаются в составе маркера проверки подлинности) и успешные федеративные входы в настоящее время включаются в журналы входов.</span><span class="sxs-lookup"><span data-stu-id="b7649-107">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="b7649-108">Последние входы возвращаются первыми.</span><span class="sxs-lookup"><span data-stu-id="b7649-108">The most recent signIns are returned first.</span></span>


## <a name="permissions"></a><span data-ttu-id="b7649-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7649-109">Permissions</span></span>
<span data-ttu-id="b7649-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7649-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7649-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7649-112">Permission type</span></span>      | <span data-ttu-id="b7649-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7649-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7649-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7649-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b7649-115">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7649-115">AuditLog.Read.All</span></span> |
|<span data-ttu-id="b7649-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7649-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7649-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b7649-117">Not supported</span></span>   |
|<span data-ttu-id="b7649-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7649-118">Application</span></span> | <span data-ttu-id="b7649-119">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7649-119">AuditLog.Read.All</span></span> | 

<span data-ttu-id="b7649-120">Кроме того, приложения должны быть [правильно зарегистрированы](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b7649-120">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="b7649-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7649-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b7649-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b7649-122">Optional query parameters</span></span>
<span data-ttu-id="b7649-123">Этот метод поддерживает указанные ниже параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b7649-123">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="b7649-124">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="b7649-124">Check [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) for how to use these parameters.</span></span>

|<span data-ttu-id="b7649-125">Имя</span><span class="sxs-lookup"><span data-stu-id="b7649-125">Name</span></span>     |<span data-ttu-id="b7649-126">Описание</span><span class="sxs-lookup"><span data-stu-id="b7649-126">Description</span></span>                            |<span data-ttu-id="b7649-127">Пример</span><span class="sxs-lookup"><span data-stu-id="b7649-127">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="b7649-128">$filter</span><span class="sxs-lookup"><span data-stu-id="b7649-128">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="b7649-129">Фильтрует результаты (строки).</span><span class="sxs-lookup"><span data-stu-id="b7649-129">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="b7649-130">$top</span><span class="sxs-lookup"><span data-stu-id="b7649-130">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="b7649-131">Задает размер страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="b7649-131">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="b7649-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="b7649-132">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="b7649-133">Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц.</span><span class="sxs-lookup"><span data-stu-id="b7649-133">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="b7649-134">Список атрибутов, поддерживаемых параметром $filter</span><span class="sxs-lookup"><span data-stu-id="b7649-134">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="b7649-135">Имя атрибута</span><span class="sxs-lookup"><span data-stu-id="b7649-135">Attribute Name</span></span> |<span data-ttu-id="b7649-136">Поддерживаемые операторы</span><span class="sxs-lookup"><span data-stu-id="b7649-136">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="b7649-137">id</span><span class="sxs-lookup"><span data-stu-id="b7649-137">id</span></span>|<span data-ttu-id="b7649-138">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-138">eq</span></span>|
|<span data-ttu-id="b7649-139">userId</span><span class="sxs-lookup"><span data-stu-id="b7649-139">userId</span></span>|<span data-ttu-id="b7649-140">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-140">eq</span></span>|
|<span data-ttu-id="b7649-141">appId</span><span class="sxs-lookup"><span data-stu-id="b7649-141">appId</span></span>|<span data-ttu-id="b7649-142">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-142">eq</span></span>|
|<span data-ttu-id="b7649-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b7649-143">createdDateTime</span></span>| <span data-ttu-id="b7649-144">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="b7649-144">eq, ge, le</span></span>|
|<span data-ttu-id="b7649-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b7649-145">userDisplayName</span></span>| <span data-ttu-id="b7649-146">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="b7649-146">eq, startswith</span></span>|
|<span data-ttu-id="b7649-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b7649-147">userPrincipalName</span></span>| <span data-ttu-id="b7649-148">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="b7649-148">eq, startswith</span></span>|
|<span data-ttu-id="b7649-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="b7649-149">appDisplayName</span></span>| <span data-ttu-id="b7649-150">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="b7649-150">eq, startswith</span></span>|
|<span data-ttu-id="b7649-151">ipAddress</span><span class="sxs-lookup"><span data-stu-id="b7649-151">ipAddress</span></span>| <span data-ttu-id="b7649-152">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="b7649-152">eq, startswith</span></span>|
|<span data-ttu-id="b7649-153">location/city</span><span class="sxs-lookup"><span data-stu-id="b7649-153">location/city</span></span>| <span data-ttu-id="b7649-154">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="b7649-154">eq, startswith</span></span>|
|<span data-ttu-id="b7649-155">location/state</span><span class="sxs-lookup"><span data-stu-id="b7649-155">location/state</span></span>| <span data-ttu-id="b7649-156">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="b7649-156">eq, startswith</span></span>|
|<span data-ttu-id="b7649-157">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="b7649-157">location/countryOrRegion</span></span>| <span data-ttu-id="b7649-158">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="b7649-158">eq, startswith</span></span>|
|<span data-ttu-id="b7649-159">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="b7649-159">status/errorCode</span></span>|<span data-ttu-id="b7649-160">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-160">eq</span></span>|
|<span data-ttu-id="b7649-161">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="b7649-161">initiatedBy/user/id</span></span>|<span data-ttu-id="b7649-162">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-162">eq</span></span>|
|<span data-ttu-id="b7649-163">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="b7649-163">initiatedBy/user/displayName</span></span>| <span data-ttu-id="b7649-164">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-164">eq</span></span>|
|<span data-ttu-id="b7649-165">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b7649-165">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="b7649-166">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="b7649-166">eq, startswith</span></span>|
|<span data-ttu-id="b7649-167">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="b7649-167">clientAppUsed</span></span>| <span data-ttu-id="b7649-168">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-168">eq</span></span>|
|<span data-ttu-id="b7649-169">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="b7649-169">conditionalAccessStatus</span></span> | <span data-ttu-id="b7649-170">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-170">eq</span></span>|
|<span data-ttu-id="b7649-171">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="b7649-171">deviceDetail/browser</span></span>| <span data-ttu-id="b7649-172">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="b7649-172">eq, startswith</span></span>|
|<span data-ttu-id="b7649-173">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="b7649-173">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="b7649-174">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="b7649-174">eq, startswith</span></span>|
|<span data-ttu-id="b7649-175">correlationId</span><span class="sxs-lookup"><span data-stu-id="b7649-175">correlationId</span></span>| <span data-ttu-id="b7649-176">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-176">eq</span></span>|
|<span data-ttu-id="b7649-177">riskDetail</span><span class="sxs-lookup"><span data-stu-id="b7649-177">riskDetail</span></span>| <span data-ttu-id="b7649-178">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-178">eq</span></span>|
|<span data-ttu-id="b7649-179">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="b7649-179">riskLevelAggregated</span></span>| <span data-ttu-id="b7649-180">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-180">eq</span></span>|
|<span data-ttu-id="b7649-181">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="b7649-181">riskLevelDuringSignIn</span></span>| <span data-ttu-id="b7649-182">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-182">eq</span></span>|
|<span data-ttu-id="b7649-183">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="b7649-183">riskEventTypes</span></span>| <span data-ttu-id="b7649-184">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-184">eq</span></span>|
|<span data-ttu-id="b7649-185">riskState</span><span class="sxs-lookup"><span data-stu-id="b7649-185">riskState</span></span>| <span data-ttu-id="b7649-186">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-186">eq</span></span>|
|<span data-ttu-id="b7649-187">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="b7649-187">originalRequestId</span></span>| <span data-ttu-id="b7649-188">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-188">eq</span></span>|
|<span data-ttu-id="b7649-189">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="b7649-189">tokenIssuerName</span></span>| <span data-ttu-id="b7649-190">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-190">eq</span></span>|
|<span data-ttu-id="b7649-191">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="b7649-191">tokenIssuerType</span></span>| <span data-ttu-id="b7649-192">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-192">eq</span></span>|
|<span data-ttu-id="b7649-193">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b7649-193">resourceDisplayName</span></span>| <span data-ttu-id="b7649-194">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-194">eq</span></span>|
|<span data-ttu-id="b7649-195">resourceId</span><span class="sxs-lookup"><span data-stu-id="b7649-195">resourceId</span></span>| <span data-ttu-id="b7649-196">eq</span><span class="sxs-lookup"><span data-stu-id="b7649-196">eq</span></span>|


## <a name="response"></a><span data-ttu-id="b7649-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7649-197">Response</span></span>
<span data-ttu-id="b7649-198">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b7649-198">If successful, this method returns a `200 OK` response code and collection of [directoryAudit](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b7649-199">Пример</span><span class="sxs-lookup"><span data-stu-id="b7649-199">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7649-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7649-200">Request</span></span>
<span data-ttu-id="b7649-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7649-201">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a><span data-ttu-id="b7649-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7649-202">Response</span></span>
<span data-ttu-id="b7649-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7649-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
