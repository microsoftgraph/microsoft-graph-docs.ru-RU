---
title: Перечисление входов
description: Описывает метод списка ресурса signIn (сущности) из API Microsoft Graph.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 5bbd66efa246a0c3bbfdabe4a083a74443486ad2
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129455"
---
# <a name="list-signins"></a><span data-ttu-id="e0548-103">Перечисление входов</span><span class="sxs-lookup"><span data-stu-id="e0548-103">List signIns</span></span>

<span data-ttu-id="e0548-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0548-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e0548-105">Получает входы пользователей Azure AD для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0548-105">Retrieve the Azure AD user sign-ins for your tenant.</span></span> <span data-ttu-id="e0548-106">Входы, которые являются интерактивными по своей природе (где имя пользователя/пароль передается как часть маркера auth) и успешные федеративные входы в настоящее время включены в журналы входа.</span><span class="sxs-lookup"><span data-stu-id="e0548-106">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span> <span data-ttu-id="e0548-107">Максимальный и по умолчанию размер страницы — 1000 объектов, и по умолчанию самые последние входы возвращаются первыми.</span><span class="sxs-lookup"><span data-stu-id="e0548-107">The maximum and default page size is 1,000 objects and by default, the most recent sign-ins are returned first.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0548-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0548-108">Permissions</span></span>

<span data-ttu-id="e0548-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="e0548-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="e0548-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0548-111">Permission type</span></span>      | <span data-ttu-id="e0548-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0548-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0548-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0548-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e0548-114">AuditLog.Read.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0548-114">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="e0548-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0548-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0548-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e0548-116">Not supported</span></span>   |
|<span data-ttu-id="e0548-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e0548-117">Application</span></span> | <span data-ttu-id="e0548-118">AuditLog.Read.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0548-118">AuditLog.Read.All and Directory.Read.All</span></span>  |

<span data-ttu-id="e0548-119">Приложения должны быть [правильно зарегистрированы в](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e0548-119">Apps must be [properly registered](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

<span data-ttu-id="e0548-120">Помимо делегирования разрешений, пользователю, входиму в который, необходимо принадлежать к одной из следующих ролей каталога, которая позволяет ему читать отчеты о входе.</span><span class="sxs-lookup"><span data-stu-id="e0548-120">In addition to the delegated permissions, the signed-in user needs to belong to one of the following directory roles that allow them to read sign-in reports.</span></span> <span data-ttu-id="e0548-121">Дополнительные информацию о роли каталогов см. в встроенной роли [Azure AD:](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="e0548-121">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="e0548-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="e0548-122">Global Administrator</span></span>
+ <span data-ttu-id="e0548-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="e0548-123">Global Reader</span></span>
+ <span data-ttu-id="e0548-124">Читатель отчетов</span><span class="sxs-lookup"><span data-stu-id="e0548-124">Reports Reader</span></span>
+ <span data-ttu-id="e0548-125">"Администратор безопасности"</span><span class="sxs-lookup"><span data-stu-id="e0548-125">Security Administrator</span></span>
+ <span data-ttu-id="e0548-126">Оператор безопасности</span><span class="sxs-lookup"><span data-stu-id="e0548-126">Security Operator</span></span>
+ <span data-ttu-id="e0548-127">Читатель сведений о безопасности</span><span class="sxs-lookup"><span data-stu-id="e0548-127">Security Reader</span></span>

## <a name="http-request"></a><span data-ttu-id="e0548-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0548-128">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0548-129">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="e0548-129">Optional query parameters</span></span>

<span data-ttu-id="e0548-130">Этот метод поддерживает `$top` параметры `$skiptoken` запроса OData и OData для настройки `$filter` ответа.</span><span class="sxs-lookup"><span data-stu-id="e0548-130">This method supports the `$top`, `$skiptoken`, and `$filter` OData Query Parameters to help customize the response.</span></span> <span data-ttu-id="e0548-131">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="e0548-131">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="response"></a><span data-ttu-id="e0548-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0548-132">Response</span></span>

<span data-ttu-id="e0548-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e0548-133">If successful, this method returns a `200 OK` response code and collection of [signIn](../resources/signin.md) objects in the response body.</span></span> <span data-ttu-id="e0548-134">Коллекция объектов указана в порядке убывания на основе **createdDateTime.**</span><span class="sxs-lookup"><span data-stu-id="e0548-134">The collection of objects is listed in descending order based on **createdDateTime**.</span></span>

## <a name="examples"></a><span data-ttu-id="e0548-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="e0548-135">Examples</span></span>

### <a name="example-1-list-all-sign-ins"></a><span data-ttu-id="e0548-136">Пример 1. Список всех входов</span><span class="sxs-lookup"><span data-stu-id="e0548-136">Example 1: List all sign-ins</span></span>

#### <a name="request"></a><span data-ttu-id="e0548-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0548-137">Request</span></span>

<span data-ttu-id="e0548-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0548-138">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e0548-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0548-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_signins"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns
```
# <a name="c"></a>[<span data-ttu-id="e0548-140">C#</span><span class="sxs-lookup"><span data-stu-id="e0548-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-signins-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0548-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0548-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-signins-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0548-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0548-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-signins-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0548-143">Java</span><span class="sxs-lookup"><span data-stu-id="e0548-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-signins-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e0548-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0548-144">Response</span></span>

<span data-ttu-id="e0548-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e0548-145">Here is an example of the response.</span></span>
><span data-ttu-id="e0548-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e0548-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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

### <a name="example-2-retrieve-the-first-10-sign-ins-to-apps-with-the-appdisplayname-that-starts-with-graph"></a><span data-ttu-id="e0548-147">Пример 2. Извлечение первых 10 входов в приложения с appDisplayName, которое начинается с "Graph"</span><span class="sxs-lookup"><span data-stu-id="e0548-147">Example 2: Retrieve the first 10 sign-ins to apps with the appDisplayName that starts with 'Graph'</span></span>

#### <a name="request"></a><span data-ttu-id="e0548-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0548-148">Request</span></span>

<span data-ttu-id="e0548-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0548-149">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns?&$filter=startsWith(appDisplayName,'Graph')&top=10
```

#### <a name="response"></a><span data-ttu-id="e0548-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0548-150">Response</span></span>

<span data-ttu-id="e0548-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e0548-151">Here is an example of the response.</span></span> <span data-ttu-id="e0548-152">Ответ включает свойство, содержаное URL-адрес, который можно использовать для получения `@odata.nextLink` следующих 10 результатов.</span><span class="sxs-lookup"><span data-stu-id="e0548-152">The response includes a `@odata.nextLink` property which contains a URL that can be used to retrieve the next 10 results.</span></span>
><span data-ttu-id="e0548-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e0548-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/auditLogs/signins?$filter=startsWith(appDisplayName%2c%27Graph%27)&$top=10&$skiptoken=70f66c0893886b49370ffdb44cd8d137b1a12b9ba02f34a16f33c5e0f7c42fc7",
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

