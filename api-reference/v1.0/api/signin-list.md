---
title: Перечисление входов
description: Описывает метод списка ресурса signIn (сущности) из API Microsoft Graph.
localization_priority: Normal
author: besiler
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 56a66140da750edc44408ecf5f06c0905e9bafe8
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910712"
---
# <a name="list-signins"></a><span data-ttu-id="e1d6a-103">Перечисление входов</span><span class="sxs-lookup"><span data-stu-id="e1d6a-103">List signIns</span></span>

<span data-ttu-id="e1d6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1d6a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1d6a-105">Получает входы пользователей Azure AD для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1d6a-105">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="e1d6a-106">В настоящее время в журналы входа включаются интерактивные входы, которые являются интерактивными (когда имя пользователя или пароль передается в рамках маркера авторизования), а успешные федеративные входы включаются в журналы входа.</span><span class="sxs-lookup"><span data-stu-id="e1d6a-106">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1d6a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1d6a-107">Permissions</span></span>

<span data-ttu-id="e1d6a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="e1d6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="e1d6a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1d6a-110">Permission type</span></span>      | <span data-ttu-id="e1d6a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1d6a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1d6a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1d6a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e1d6a-113">AuditLog.Read.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1d6a-113">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="e1d6a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1d6a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1d6a-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e1d6a-115">Not supported</span></span>   |
|<span data-ttu-id="e1d6a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1d6a-116">Application</span></span> | <span data-ttu-id="e1d6a-117">AuditLog.Read.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e1d6a-117">AuditLog.Read.All and Directory.Read.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="e1d6a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1d6a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1d6a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e1d6a-119">Optional query parameters</span></span>

<span data-ttu-id="e1d6a-120">Этот метод поддерживает следующие параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e1d6a-120">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="e1d6a-121">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="e1d6a-121">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

|<span data-ttu-id="e1d6a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e1d6a-122">Name</span></span>     |<span data-ttu-id="e1d6a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e1d6a-123">Description</span></span>                            |<span data-ttu-id="e1d6a-124">Пример</span><span class="sxs-lookup"><span data-stu-id="e1d6a-124">Example</span></span>|
|:--------------------|----------------|------------------------------------------------------------------------|
|[<span data-ttu-id="e1d6a-125">$filter</span><span class="sxs-lookup"><span data-stu-id="e1d6a-125">$filter</span></span>](/graph/query_parameters#filter-parameter)|<span data-ttu-id="e1d6a-126">Фильтрует результаты (строки).</span><span class="sxs-lookup"><span data-stu-id="e1d6a-126">Filters results (rows).</span></span> |`/auditLogs/signIns?&$filter=createdDateTime le 2018-01-24`
|[<span data-ttu-id="e1d6a-127">$top</span><span class="sxs-lookup"><span data-stu-id="e1d6a-127">$top</span></span>](/graph/query_parameters#top-parameter)|<span data-ttu-id="e1d6a-128">Задает размер страницы результатов.</span><span class="sxs-lookup"><span data-stu-id="e1d6a-128">Sets the page size of results.</span></span>|`/auditLogs/signIns?$top=1`|
|[<span data-ttu-id="e1d6a-129">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="e1d6a-129">$skiptoken</span></span>](/graph/query_parameters#skiptoken-parameter)|<span data-ttu-id="e1d6a-130">Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц.</span><span class="sxs-lookup"><span data-stu-id="e1d6a-130">Retrieves the next page of results from result sets that span multiple pages.</span></span>|`/auditLogs/signIns?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="attributes-supported-by-filter-parameter"></a><span data-ttu-id="e1d6a-131">Атрибуты, поддерживаемые $filter параметра</span><span class="sxs-lookup"><span data-stu-id="e1d6a-131">Attributes supported by $filter parameter</span></span>

|<span data-ttu-id="e1d6a-132">Имя атрибута</span><span class="sxs-lookup"><span data-stu-id="e1d6a-132">Attribute name</span></span> |<span data-ttu-id="e1d6a-133">Поддерживаемые операторы</span><span class="sxs-lookup"><span data-stu-id="e1d6a-133">Supported operators</span></span>|
|:----------------|:------|
|<span data-ttu-id="e1d6a-134">id</span><span class="sxs-lookup"><span data-stu-id="e1d6a-134">id</span></span>|<span data-ttu-id="e1d6a-135">eq</span><span class="sxs-lookup"><span data-stu-id="e1d6a-135">eq</span></span>|
|<span data-ttu-id="e1d6a-136">userId</span><span class="sxs-lookup"><span data-stu-id="e1d6a-136">userId</span></span>|<span data-ttu-id="e1d6a-137">eq</span><span class="sxs-lookup"><span data-stu-id="e1d6a-137">eq</span></span>|
|<span data-ttu-id="e1d6a-138">appId</span><span class="sxs-lookup"><span data-stu-id="e1d6a-138">appId</span></span>|<span data-ttu-id="e1d6a-139">eq</span><span class="sxs-lookup"><span data-stu-id="e1d6a-139">eq</span></span>|
|<span data-ttu-id="e1d6a-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1d6a-140">createdDateTime</span></span>| <span data-ttu-id="e1d6a-141">eq, le, ge</span><span class="sxs-lookup"><span data-stu-id="e1d6a-141">eq, le, ge</span></span>|
|<span data-ttu-id="e1d6a-142">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e1d6a-142">userDisplayName</span></span>| <span data-ttu-id="e1d6a-143">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="e1d6a-143">eq, startswith</span></span>|
|<span data-ttu-id="e1d6a-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e1d6a-144">userPrincipalName</span></span>| <span data-ttu-id="e1d6a-145">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="e1d6a-145">eq, startswith</span></span>|
|<span data-ttu-id="e1d6a-146">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="e1d6a-146">appDisplayName</span></span>| <span data-ttu-id="e1d6a-147">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="e1d6a-147">eq, startswith</span></span>|
|<span data-ttu-id="e1d6a-148">ipAddress</span><span class="sxs-lookup"><span data-stu-id="e1d6a-148">ipAddress</span></span>| <span data-ttu-id="e1d6a-149">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="e1d6a-149">eq, startswith</span></span>|
|<span data-ttu-id="e1d6a-150">location/city</span><span class="sxs-lookup"><span data-stu-id="e1d6a-150">location/city</span></span>| <span data-ttu-id="e1d6a-151">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="e1d6a-151">eq, startswith</span></span>|
|<span data-ttu-id="e1d6a-152">location/state</span><span class="sxs-lookup"><span data-stu-id="e1d6a-152">location/state</span></span>| <span data-ttu-id="e1d6a-153">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="e1d6a-153">eq, startswith</span></span>|
|<span data-ttu-id="e1d6a-154">location/countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="e1d6a-154">location/countryOrRegion</span></span>| <span data-ttu-id="e1d6a-155">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="e1d6a-155">eq, startswith</span></span>|
|<span data-ttu-id="e1d6a-156">status/errorCode</span><span class="sxs-lookup"><span data-stu-id="e1d6a-156">status/errorCode</span></span>|<span data-ttu-id="e1d6a-157">eq</span><span class="sxs-lookup"><span data-stu-id="e1d6a-157">eq</span></span>|
|<span data-ttu-id="e1d6a-158">initiatedBy/user/id</span><span class="sxs-lookup"><span data-stu-id="e1d6a-158">initiatedBy/user/id</span></span>|<span data-ttu-id="e1d6a-159">eq</span><span class="sxs-lookup"><span data-stu-id="e1d6a-159">eq</span></span>|
|<span data-ttu-id="e1d6a-160">initiatedBy/user/displayName</span><span class="sxs-lookup"><span data-stu-id="e1d6a-160">initiatedBy/user/displayName</span></span>| <span data-ttu-id="e1d6a-161">eq</span><span class="sxs-lookup"><span data-stu-id="e1d6a-161">eq</span></span>|
|<span data-ttu-id="e1d6a-162">initiatedBy/user/userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e1d6a-162">initiatedBy/user/userPrincipalName</span></span>| <span data-ttu-id="e1d6a-163">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="e1d6a-163">eq, startswith</span></span>|
|<span data-ttu-id="e1d6a-164">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="e1d6a-164">clientAppUsed</span></span>| <span data-ttu-id="e1d6a-165">eq</span><span class="sxs-lookup"><span data-stu-id="e1d6a-165">eq</span></span>|
|<span data-ttu-id="e1d6a-166">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="e1d6a-166">conditionalAccessStatus</span></span> | <span data-ttu-id="e1d6a-167">eq</span><span class="sxs-lookup"><span data-stu-id="e1d6a-167">eq</span></span>|
|<span data-ttu-id="e1d6a-168">deviceDetail/browser</span><span class="sxs-lookup"><span data-stu-id="e1d6a-168">deviceDetail/browser</span></span>| <span data-ttu-id="e1d6a-169">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="e1d6a-169">eq, startswith</span></span>|
|<span data-ttu-id="e1d6a-170">deviceDetail/operatingSystem</span><span class="sxs-lookup"><span data-stu-id="e1d6a-170">deviceDetail/operatingSystem</span></span>| <span data-ttu-id="e1d6a-171">eq, startswith</span><span class="sxs-lookup"><span data-stu-id="e1d6a-171">eq, startswith</span></span>|
|<span data-ttu-id="e1d6a-172">correlationId</span><span class="sxs-lookup"><span data-stu-id="e1d6a-172">correlationId</span></span>| <span data-ttu-id="e1d6a-173">eq</span><span class="sxs-lookup"><span data-stu-id="e1d6a-173">eq</span></span>|

## <a name="response"></a><span data-ttu-id="e1d6a-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1d6a-174">Response</span></span>

<span data-ttu-id="e1d6a-175">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1d6a-175">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1d6a-176">Пример</span><span class="sxs-lookup"><span data-stu-id="e1d6a-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1d6a-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1d6a-177">Request</span></span>

<span data-ttu-id="e1d6a-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1d6a-178">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e1d6a-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1d6a-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_signins"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="e1d6a-180">C#</span><span class="sxs-lookup"><span data-stu-id="e1d6a-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1d6a-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1d6a-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1d6a-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1d6a-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1d6a-183">Java</span><span class="sxs-lookup"><span data-stu-id="e1d6a-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-signins-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e1d6a-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1d6a-184">Response</span></span>

<span data-ttu-id="e1d6a-185">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e1d6a-185">Here is an example of the response.</span></span>
><span data-ttu-id="e1d6a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1d6a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/auditLogs/signIns?$top=1&$skiptoken=9177f2e3532fcd4c4d225f68f7b9bdf7_1",
    "value": [
        {
            "id": "66ea54eb-6301-4ee5-be62-ff5a759b0100",
            "createdDateTime": "2020-03-13T19:15:41.6195833Z",
            "userDisplayName": "Test Contoso",
            "userPrincipalName": "testaccount1@contoso.com",
            "userId": "26be570a-ae82-4189-b4e2-a37c6808512d",
            "appId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "appDisplayName": "Graph explorer",
            "ipAddress": "131.107.159.37",
            "clientAppUsed": "Browser",
            "correlationId": "d79f5bee-5860-4832-928f-3133e22ae912",
            "conditionalAccessStatus": "notApplied",
            "isInteractive": true,
            "riskDetail": "none",
            "riskLevelAggregated": "none",
            "riskLevelDuringSignIn": "none",
            "riskState": "none",
            "riskEventTypes": [],
            "resourceDisplayName": "Microsoft Graph",
            "resourceId": "00000003-0000-0000-c000-000000000000",
            "status": {
                "errorCode": 0,
                "failureReason": null,
                "additionalDetails": null
            },
            "deviceDetail": {
                "deviceId": "",
                "displayName": null,
                "operatingSystem": "Windows 10",
                "browser": "Edge 80.0.361",
                "isCompliant": null,
                "isManaged": null,
                "trustType": null
            },
            "location": {
                "city": "Redmond",
                "state": "Washington",
                "countryOrRegion": "US",
                "geoCoordinates": {
                    "altitude": null,
                    "latitude": 47.68050003051758,
                    "longitude": -122.12094116210938
                }
            },
            "appliedConditionalAccessPolicies": [
                {
                    "id": "de7e60eb-ed89-4d73-8205-2227def6b7c9",
                    "displayName": "SharePoint limited access for guest workers",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled"
                },
                {
                    "id": "6701123a-b4c6-48af-8565-565c8bf7cabc",
                    "displayName": "Medium signin risk block",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled"
                },
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

