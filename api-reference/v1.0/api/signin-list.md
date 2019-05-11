---
title: Перечисление входов
description: Описывает метод List ресурса SignIn (Entity) из API Microsoft Graph.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1c5d4f2d7bc4e60eb0b1d1d876e4c9bf5000a35c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951433"
---
# <a name="list-signins"></a><span data-ttu-id="5ea84-103">Перечисление входов</span><span class="sxs-lookup"><span data-stu-id="5ea84-103">List signIns</span></span>

<span data-ttu-id="5ea84-104">Получает входы пользователей Azure AD для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ea84-104">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="5ea84-105">Интерактивные входы в природе (при условии, что имя пользователя и пароль передаются в составе маркера проверки подлинности); успешные Федеративные входы в систему в данный момент включены в журналы входа.</span><span class="sxs-lookup"><span data-stu-id="5ea84-105">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ea84-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ea84-106">Permissions</span></span>

<span data-ttu-id="5ea84-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="5ea84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="5ea84-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ea84-109">Permission type</span></span>      | <span data-ttu-id="5ea84-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ea84-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ea84-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ea84-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5ea84-112">Аудитлог. Read. ALL и Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="5ea84-112">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="5ea84-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ea84-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ea84-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5ea84-114">Not supported</span></span>   |
|<span data-ttu-id="5ea84-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ea84-115">Application</span></span> | <span data-ttu-id="5ea84-116">AuditLog.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ea84-116">AuditLog.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ea84-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ea84-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ea84-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5ea84-118">Optional query parameters</span></span>

<span data-ttu-id="5ea84-119">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5ea84-119">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="5ea84-120">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="5ea84-120">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="5ea84-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5ea84-121">Name</span></span>     |<span data-ttu-id="5ea84-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5ea84-122">Description</span></span>                            |<span data-ttu-id="5ea84-123">Пример</span><span class="sxs-lookup"><span data-stu-id="5ea84-123">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="5ea84-124">$filter</span><span class="sxs-lookup"><span data-stu-id="5ea84-124">$filter</span></span>](/graph/query_parameters#filter-parameter)|<span data-ttu-id="5ea84-125">Фильтрует результаты (строки).</span><span class="sxs-lookup"><span data-stu-id="5ea84-125">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="5ea84-126">$top</span><span class="sxs-lookup"><span data-stu-id="5ea84-126">$top</span></span>](/graph/query_parameters#top-parameter)|<span data-ttu-id="5ea84-127">Задает размер страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="5ea84-127">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="5ea84-128">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="5ea84-128">$skiptoken</span></span>](/graph/query_parameters#skiptoken-parameter)|<span data-ttu-id="5ea84-129">Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц.</span><span class="sxs-lookup"><span data-stu-id="5ea84-129">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="5ea84-130">Атрибуты, поддерживаемые параметром $filter</span><span class="sxs-lookup"><span data-stu-id="5ea84-130">Attributes supported by $filter parameter</span></span>

|<span data-ttu-id="5ea84-131">Имя атрибута</span><span class="sxs-lookup"><span data-stu-id="5ea84-131">Attribute name</span></span> |<span data-ttu-id="5ea84-132">Поддерживаемые операторы</span><span class="sxs-lookup"><span data-stu-id="5ea84-132">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="5ea84-133">id</span><span class="sxs-lookup"><span data-stu-id="5ea84-133">id</span></span>|<span data-ttu-id="5ea84-134">eq</span><span class="sxs-lookup"><span data-stu-id="5ea84-134">eq</span></span>|
|<span data-ttu-id="5ea84-135">userId</span><span class="sxs-lookup"><span data-stu-id="5ea84-135">userId</span></span>|<span data-ttu-id="5ea84-136">eq</span><span class="sxs-lookup"><span data-stu-id="5ea84-136">eq</span></span>|
|<span data-ttu-id="5ea84-137">appId</span><span class="sxs-lookup"><span data-stu-id="5ea84-137">appId</span></span>|<span data-ttu-id="5ea84-138">eq</span><span class="sxs-lookup"><span data-stu-id="5ea84-138">eq</span></span>|
|<span data-ttu-id="5ea84-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ea84-139">createdDateTime</span></span>| <span data-ttu-id="5ea84-140">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="5ea84-140">eq, le, ge</span></span>|
|<span data-ttu-id="5ea84-141">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5ea84-141">userDisplayName</span></span>| <span data-ttu-id="5ea84-142">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="5ea84-142">eq, startswith</span></span>|
|<span data-ttu-id="5ea84-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5ea84-143">userPrincipalName</span></span>| <span data-ttu-id="5ea84-144">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="5ea84-144">eq, startswith</span></span>|
|<span data-ttu-id="5ea84-145">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="5ea84-145">appDisplayName</span></span>| <span data-ttu-id="5ea84-146">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="5ea84-146">eq, startswith</span></span>|
|<span data-ttu-id="5ea84-147">ipAddress</span><span class="sxs-lookup"><span data-stu-id="5ea84-147">ipAddress</span></span>| <span data-ttu-id="5ea84-148">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="5ea84-148">eq, startswith</span></span>|
|<span data-ttu-id="5ea84-149">location/city</span><span class="sxs-lookup"><span data-stu-id="5ea84-149">location/city</span></span>| <span data-ttu-id="5ea84-150">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="5ea84-150">eq, startswith</span></span>|
|<span data-ttu-id="5ea84-151">location/state</span><span class="sxs-lookup"><span data-stu-id="5ea84-151">location/state</span></span>| <span data-ttu-id="5ea84-152">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="5ea84-152">eq, startswith</span></span>|
|<span data-ttu-id="5ea84-153">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="5ea84-153">location/countryOrRegion</span></span>| <span data-ttu-id="5ea84-154">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="5ea84-154">eq, startswith</span></span>|
|<span data-ttu-id="5ea84-155">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="5ea84-155">status/errorCode</span></span>|<span data-ttu-id="5ea84-156">eq</span><span class="sxs-lookup"><span data-stu-id="5ea84-156">eq</span></span>|
|<span data-ttu-id="5ea84-157">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="5ea84-157">initiatedBy/user/id</span></span>|<span data-ttu-id="5ea84-158">eq</span><span class="sxs-lookup"><span data-stu-id="5ea84-158">eq</span></span>|
|<span data-ttu-id="5ea84-159">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="5ea84-159">initiatedBy/user/displayName</span></span>| <span data-ttu-id="5ea84-160">eq</span><span class="sxs-lookup"><span data-stu-id="5ea84-160">eq</span></span>|
|<span data-ttu-id="5ea84-161">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5ea84-161">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="5ea84-162">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="5ea84-162">eq, startswith</span></span>|
|<span data-ttu-id="5ea84-163">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="5ea84-163">clientAppUsed</span></span>| <span data-ttu-id="5ea84-164">eq</span><span class="sxs-lookup"><span data-stu-id="5ea84-164">eq</span></span>|
|<span data-ttu-id="5ea84-165">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="5ea84-165">conditionalAccessStatus</span></span> | <span data-ttu-id="5ea84-166">eq</span><span class="sxs-lookup"><span data-stu-id="5ea84-166">eq</span></span>|
|<span data-ttu-id="5ea84-167">Девицедетаилс и браузер</span><span class="sxs-lookup"><span data-stu-id="5ea84-167">deviceDetails/browser</span></span>| <span data-ttu-id="5ea84-168">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="5ea84-168">eq, startswith</span></span>|
|<span data-ttu-id="5ea84-169">Девицедетаилс и операционной операционной</span><span class="sxs-lookup"><span data-stu-id="5ea84-169">deviceDetails/operatingSystem</span></span>| <span data-ttu-id="5ea84-170">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="5ea84-170">eq, startswith</span></span>|
|<span data-ttu-id="5ea84-171">correlationId</span><span class="sxs-lookup"><span data-stu-id="5ea84-171">correlationId</span></span>| <span data-ttu-id="5ea84-172">eq</span><span class="sxs-lookup"><span data-stu-id="5ea84-172">eq</span></span>|
|<span data-ttu-id="5ea84-173">Риск</span><span class="sxs-lookup"><span data-stu-id="5ea84-173">isRisky</span></span>| <span data-ttu-id="5ea84-174">eq</span><span class="sxs-lookup"><span data-stu-id="5ea84-174">eq</span></span>|

## <a name="response"></a><span data-ttu-id="5ea84-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ea84-175">Response</span></span>

<span data-ttu-id="5ea84-176">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5ea84-176">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ea84-177">Пример</span><span class="sxs-lookup"><span data-stu-id="5ea84-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ea84-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ea84-178">Request</span></span>

<span data-ttu-id="5ea84-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ea84-179">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_signins"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs/signIns
```

### <a name="response"></a><span data-ttu-id="5ea84-180">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ea84-180">Response</span></span>

<span data-ttu-id="5ea84-181">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5ea84-181">Here is an example of the response.</span></span>
><span data-ttu-id="5ea84-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5ea84-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5ea84-184">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="5ea84-184">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5ea84-185">C#</span><span class="sxs-lookup"><span data-stu-id="5ea84-185">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list_signins-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5ea84-186">Javascript</span><span class="sxs-lookup"><span data-stu-id="5ea84-186">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list_signins-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

```json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
    "value": [{
        "id": "id",
        "appId": "d3590ed6-52b3-4102-aeff-aad2292ab01c",
        "appDisplayName": "Azure",
        "createdDateTime": "2018-01-09T21:17:21.5077253Z",
        "clientAppUsed": null,
        "conditionalAccessApplied": true,
        "conditionalAccessPolicies": [{
            "id": "26490ed6-52b3-4102-aeff-aad2292abacf",
            "displayName": "capPolicy",
            "enforcedAccessControls": ["MFA", "TOU"],
            "enforcedSessionControls": ["CloudAppSecurity"],
            "result": "success"
        }],
        "correlationId": "17444d3c-563d-4b08-ac20-815892b87e42",
        "deviceDetail": {
            "deviceId": "34390ed6-52b3-4102-aeff-aad2292abac3",
            "displayName": "DeviceName",
            "operatingSystem": "Windows 10",
            "browser": "Rich Client v3.14.1592.7",
            "isCompliant": true,
            "isManaged": true,
            "trustType": ""
        },
        "ipAddress": "127.0.0.1",
        "location": {
            "city": "Redmond",
            "state": "WA",
            "countryOrRegion": "USA",
            "geoCoordinates": {
                "altitude": 41.589,
                "latitude": 41.589,
                "longitude": -93.6151
            }
        },
        "status": {
            "errorCode": 0,
            "failureReason": null,
            "additionalDetails": "SignIn Success & CA Success"
        },
        "userDisplayName": "Jamie Doe",
        "userPrincipalName": "jdoe@wingtiptoys.com",
        "userId": "bbb3b4b5-e6e6-f7f5-f7f5-090805040302"
    }]
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
    "Error: /api-reference/v1.0/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/signin-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
