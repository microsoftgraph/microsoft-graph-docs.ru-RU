---
title: Получение объекта signIn
description: Описывает метод get ресурса signIn (сущности) из API Microsoft Graph.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: cb09d2f9fde80ba6e9d24cae80a39a74faacc3ed
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131994"
---
# <a name="get-signin"></a><span data-ttu-id="5bf1b-103">Получение объекта signIn</span><span class="sxs-lookup"><span data-stu-id="5bf1b-103">Get signIn</span></span>

<span data-ttu-id="5bf1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bf1b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5bf1b-105">Получение определенного события входа пользователя Azure AD для клиента.</span><span class="sxs-lookup"><span data-stu-id="5bf1b-105">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="5bf1b-106">В настоящее время в журналы входа включаются интерактивные входы, которые являются интерактивными (когда имя пользователя или пароль передается в рамках маркера авторизования), а успешные федеративные входы включаются в журналы входа.</span><span class="sxs-lookup"><span data-stu-id="5bf1b-106">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bf1b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5bf1b-107">Permissions</span></span>

<span data-ttu-id="5bf1b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="5bf1b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="5bf1b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5bf1b-110">Permission type</span></span>      | <span data-ttu-id="5bf1b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5bf1b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bf1b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5bf1b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5bf1b-113">AuditLog.Read.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bf1b-113">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="5bf1b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5bf1b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bf1b-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5bf1b-115">Not supported</span></span>   |
|<span data-ttu-id="5bf1b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5bf1b-116">Application</span></span> | <span data-ttu-id="5bf1b-117">AuditLog.Read.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bf1b-117">AuditLog.Read.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bf1b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5bf1b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5bf1b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5bf1b-119">Optional query parameters</span></span>

<span data-ttu-id="5bf1b-120">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5bf1b-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="5bf1b-121">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="5bf1b-121">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bf1b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5bf1b-122">Request headers</span></span>

| <span data-ttu-id="5bf1b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="5bf1b-123">Name</span></span>      |<span data-ttu-id="5bf1b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5bf1b-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5bf1b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5bf1b-125">Authorization</span></span>  | <span data-ttu-id="5bf1b-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5bf1b-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bf1b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5bf1b-127">Request body</span></span>

<span data-ttu-id="5bf1b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5bf1b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bf1b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bf1b-129">Response</span></span>

<span data-ttu-id="5bf1b-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5bf1b-130">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bf1b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5bf1b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bf1b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5bf1b-132">Request</span></span>

<span data-ttu-id="5bf1b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5bf1b-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5bf1b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bf1b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns/{id}
```
# <a name="c"></a>[<span data-ttu-id="5bf1b-135">C#</span><span class="sxs-lookup"><span data-stu-id="5bf1b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5bf1b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5bf1b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5bf1b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bf1b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5bf1b-138">Java</span><span class="sxs-lookup"><span data-stu-id="5bf1b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5bf1b-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="5bf1b-139">Response</span></span>

<span data-ttu-id="5bf1b-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5bf1b-140">Here is an example of the response.</span></span>
><span data-ttu-id="5bf1b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5bf1b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 211
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
  "description": "Get signIn",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

