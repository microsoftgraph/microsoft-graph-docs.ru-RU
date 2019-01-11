---
title: Список signIns
description: Извлекает Azure AD входы для клиента. Войти в систему, взаимодействующих в характер (где имя пользователя и пароль передается как часть маркера авторизации) и успешные федеративных войти в систему в данный момент включены в журналы входа.  Самые последние signIns возвращаются первые.
localization_priority: Priority
ms.openlocfilehash: 8596bd168a3e10cbea9e15e2f61d6bd668fd27b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861791"
---
# <a name="list-signins"></a><span data-ttu-id="3a5a8-105">Список signIns</span><span class="sxs-lookup"><span data-stu-id="3a5a8-105">List signIns</span></span>

<span data-ttu-id="3a5a8-106">Извлекает Azure AD входы для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a5a8-106">Retrieves the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="3a5a8-107">Войти в систему, взаимодействующих в характер (где имя пользователя и пароль передается как часть маркера авторизации) и успешные федеративных войти в систему в данный момент включены в журналы входа.</span><span class="sxs-lookup"><span data-stu-id="3a5a8-107">Sign-ins that are interactive in nature (where a username/password is passed as part of authorization token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>  <span data-ttu-id="3a5a8-108">Самые последние signIns возвращаются первые.</span><span class="sxs-lookup"><span data-stu-id="3a5a8-108">The most recent signIns are returned first.</span></span>


## <a name="permissions"></a><span data-ttu-id="3a5a8-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a5a8-109">Permissions</span></span>
<span data-ttu-id="3a5a8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a5a8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a5a8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a5a8-112">Permission type</span></span>      | <span data-ttu-id="3a5a8-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a5a8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a5a8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a5a8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3a5a8-115">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a5a8-115">AuditLog.Read.All</span></span> |
|<span data-ttu-id="3a5a8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a5a8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a5a8-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="3a5a8-117">Not supported</span></span>   |
|<span data-ttu-id="3a5a8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a5a8-118">Application</span></span> | <span data-ttu-id="3a5a8-119">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a5a8-119">AuditLog.Read.All</span></span> | 

<span data-ttu-id="3a5a8-120">Кроме того приложения должны быть [правильно зарегистрирован](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) для Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3a5a8-120">In addition, apps must be [properly registered](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

## <a name="http-request"></a><span data-ttu-id="3a5a8-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a5a8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3a5a8-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3a5a8-122">Optional query parameters</span></span>
<span data-ttu-id="3a5a8-123">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3a5a8-123">This method supports the following OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="3a5a8-124">Проверьте [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для порядок использования этих параметров.</span><span class="sxs-lookup"><span data-stu-id="3a5a8-124">Check [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) for how to use these parameters.</span></span>

|<span data-ttu-id="3a5a8-125">Имя</span><span class="sxs-lookup"><span data-stu-id="3a5a8-125">Name</span></span>     |<span data-ttu-id="3a5a8-126">Описание</span><span class="sxs-lookup"><span data-stu-id="3a5a8-126">Description</span></span>                            |<span data-ttu-id="3a5a8-127">Пример</span><span class="sxs-lookup"><span data-stu-id="3a5a8-127">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="3a5a8-128">$filter</span><span class="sxs-lookup"><span data-stu-id="3a5a8-128">$filter</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#filter-parameter)|<span data-ttu-id="3a5a8-129">Фильтрует результаты (строки).</span><span class="sxs-lookup"><span data-stu-id="3a5a8-129">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="3a5a8-130">$top</span><span class="sxs-lookup"><span data-stu-id="3a5a8-130">$top</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#top-parameter)|<span data-ttu-id="3a5a8-131">Задает размер страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="3a5a8-131">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="3a5a8-132">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="3a5a8-132">$skiptoken</span></span>](https://developer.microsoft.com/graph/docs/concepts/query_parameters#skiptoken-parameter)|<span data-ttu-id="3a5a8-133">Извлекает следующую страницу результатов из результатов наборы данных, которые охватывают несколько страниц.</span><span class="sxs-lookup"><span data-stu-id="3a5a8-133">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a><span data-ttu-id="3a5a8-134">Список атрибутов, поддерживаемых $filter параметром</span><span class="sxs-lookup"><span data-stu-id="3a5a8-134">List of attributes supported by $filter parameter</span></span>
|<span data-ttu-id="3a5a8-135">Имя атрибута</span><span class="sxs-lookup"><span data-stu-id="3a5a8-135">Attribute Name</span></span> |<span data-ttu-id="3a5a8-136">Поддерживаемые операторы</span><span class="sxs-lookup"><span data-stu-id="3a5a8-136">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="3a5a8-137">id</span><span class="sxs-lookup"><span data-stu-id="3a5a8-137">id</span></span>|<span data-ttu-id="3a5a8-138">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-138">eq</span></span>|
|<span data-ttu-id="3a5a8-139">userId</span><span class="sxs-lookup"><span data-stu-id="3a5a8-139">userId</span></span>|<span data-ttu-id="3a5a8-140">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-140">eq</span></span>|
|<span data-ttu-id="3a5a8-141">appId</span><span class="sxs-lookup"><span data-stu-id="3a5a8-141">appId</span></span>|<span data-ttu-id="3a5a8-142">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-142">eq</span></span>|
|<span data-ttu-id="3a5a8-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a5a8-143">createdDateTime</span></span>| <span data-ttu-id="3a5a8-144">EQ, le ge</span><span class="sxs-lookup"><span data-stu-id="3a5a8-144">eq, le, ge</span></span>|
|<span data-ttu-id="3a5a8-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3a5a8-145">userDisplayName</span></span>| <span data-ttu-id="3a5a8-146">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="3a5a8-146">eq, startswith</span></span>|
|<span data-ttu-id="3a5a8-147">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3a5a8-147">userPrincipalName</span></span>| <span data-ttu-id="3a5a8-148">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="3a5a8-148">eq, startswith</span></span>|
|<span data-ttu-id="3a5a8-149">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="3a5a8-149">appDisplayName</span></span>| <span data-ttu-id="3a5a8-150">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="3a5a8-150">eq, startswith</span></span>|
|<span data-ttu-id="3a5a8-151">ipAddress</span><span class="sxs-lookup"><span data-stu-id="3a5a8-151">ipAddress</span></span>| <span data-ttu-id="3a5a8-152">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="3a5a8-152">eq, startswith</span></span>|
|<span data-ttu-id="3a5a8-153">Город /</span><span class="sxs-lookup"><span data-stu-id="3a5a8-153">location/city</span></span>| <span data-ttu-id="3a5a8-154">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="3a5a8-154">eq, startswith</span></span>|
|<span data-ttu-id="3a5a8-155">расположение/состояние</span><span class="sxs-lookup"><span data-stu-id="3a5a8-155">location/state</span></span>| <span data-ttu-id="3a5a8-156">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="3a5a8-156">eq, startswith</span></span>|
|<span data-ttu-id="3a5a8-157">расположение/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="3a5a8-157">location/countryOrRegion</span></span>| <span data-ttu-id="3a5a8-158">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="3a5a8-158">eq, startswith</span></span>|
|<span data-ttu-id="3a5a8-159">Код состояния или ошибки</span><span class="sxs-lookup"><span data-stu-id="3a5a8-159">status/errorCode</span></span>|<span data-ttu-id="3a5a8-160">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-160">eq</span></span>|
|<span data-ttu-id="3a5a8-161">initiatedBy/пользователь</span><span class="sxs-lookup"><span data-stu-id="3a5a8-161">initiatedBy/user/id</span></span>|<span data-ttu-id="3a5a8-162">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-162">eq</span></span>|
|<span data-ttu-id="3a5a8-163">initiatedBy/пользователей/displayName</span><span class="sxs-lookup"><span data-stu-id="3a5a8-163">initiatedBy/user/displayName</span></span>| <span data-ttu-id="3a5a8-164">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-164">eq</span></span>|
|<span data-ttu-id="3a5a8-165">initiatedBy/пользователей/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3a5a8-165">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="3a5a8-166">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="3a5a8-166">eq, startswith</span></span>|
|<span data-ttu-id="3a5a8-167">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="3a5a8-167">clientAppUsed</span></span>| <span data-ttu-id="3a5a8-168">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-168">eq</span></span>|
|<span data-ttu-id="3a5a8-169">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="3a5a8-169">conditionalAccessStatus</span></span> | <span data-ttu-id="3a5a8-170">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-170">eq</span></span>|
|<span data-ttu-id="3a5a8-171">deviceDetail/браузера</span><span class="sxs-lookup"><span data-stu-id="3a5a8-171">deviceDetail/browser</span></span>| <span data-ttu-id="3a5a8-172">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="3a5a8-172">eq, startswith</span></span>|
|<span data-ttu-id="3a5a8-173">deviceDetail/операционной системы</span><span class="sxs-lookup"><span data-stu-id="3a5a8-173">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="3a5a8-174">EQ, startswith</span><span class="sxs-lookup"><span data-stu-id="3a5a8-174">eq, startswith</span></span>|
|<span data-ttu-id="3a5a8-175">correlationId</span><span class="sxs-lookup"><span data-stu-id="3a5a8-175">correlationId</span></span>| <span data-ttu-id="3a5a8-176">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-176">eq</span></span>|
|<span data-ttu-id="3a5a8-177">riskDetail</span><span class="sxs-lookup"><span data-stu-id="3a5a8-177">riskDetail</span></span>| <span data-ttu-id="3a5a8-178">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-178">eq</span></span>|
|<span data-ttu-id="3a5a8-179">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="3a5a8-179">riskLevelAggregated</span></span>| <span data-ttu-id="3a5a8-180">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-180">eq</span></span>|
|<span data-ttu-id="3a5a8-181">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="3a5a8-181">riskLevelDuringSignIn</span></span>| <span data-ttu-id="3a5a8-182">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-182">eq</span></span>|
|<span data-ttu-id="3a5a8-183">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="3a5a8-183">riskEventTypes</span></span>| <span data-ttu-id="3a5a8-184">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-184">eq</span></span>|
|<span data-ttu-id="3a5a8-185">riskState</span><span class="sxs-lookup"><span data-stu-id="3a5a8-185">riskState</span></span>| <span data-ttu-id="3a5a8-186">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-186">eq</span></span>|
|<span data-ttu-id="3a5a8-187">originalRequestId</span><span class="sxs-lookup"><span data-stu-id="3a5a8-187">originalRequestId</span></span>| <span data-ttu-id="3a5a8-188">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-188">eq</span></span>|
|<span data-ttu-id="3a5a8-189">tokenIssuerName</span><span class="sxs-lookup"><span data-stu-id="3a5a8-189">tokenIssuerName</span></span>| <span data-ttu-id="3a5a8-190">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-190">eq</span></span>|
|<span data-ttu-id="3a5a8-191">tokenIssuerType</span><span class="sxs-lookup"><span data-stu-id="3a5a8-191">tokenIssuerType</span></span>| <span data-ttu-id="3a5a8-192">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-192">eq</span></span>|
|<span data-ttu-id="3a5a8-193">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="3a5a8-193">resourceDisplayName</span></span>| <span data-ttu-id="3a5a8-194">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-194">eq</span></span>|
|<span data-ttu-id="3a5a8-195">resourceId</span><span class="sxs-lookup"><span data-stu-id="3a5a8-195">resourceId</span></span>| <span data-ttu-id="3a5a8-196">eq</span><span class="sxs-lookup"><span data-stu-id="3a5a8-196">eq</span></span>|


## <a name="response"></a><span data-ttu-id="3a5a8-197">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a5a8-197">Response</span></span>
<span data-ttu-id="3a5a8-198">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [входить](../resources/signin.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3a5a8-198">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a5a8-199">Пример</span><span class="sxs-lookup"><span data-stu-id="3a5a8-199">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a5a8-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a5a8-200">Request</span></span>
<span data-ttu-id="3a5a8-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a5a8-201">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_signins"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
##### <a name="response"></a><span data-ttu-id="3a5a8-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a5a8-202">Response</span></span>
<span data-ttu-id="3a5a8-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3a5a8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
