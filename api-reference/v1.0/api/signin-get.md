---
title: Получение объекта signIn
description: Описывает метод получения ресурса signIn (сущности) из API Microsoft Graph.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 6c5e3f215409e065ce6548e59827beb8ae1eafdf
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129465"
---
# <a name="get-signin"></a><span data-ttu-id="d2f18-103">Получение объекта signIn</span><span class="sxs-lookup"><span data-stu-id="d2f18-103">Get signIn</span></span>

<span data-ttu-id="d2f18-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2f18-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d2f18-105">Получение определенного события входа пользователя Azure AD для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2f18-105">Retrieve a specific Azure AD user sign-in event for your tenant.</span></span> <span data-ttu-id="d2f18-106">Входы, которые являются интерактивными по своей природе (где имя пользователя/пароль передается как часть маркера auth) и успешные федеративные входы в настоящее время включены в журналы входа.</span><span class="sxs-lookup"><span data-stu-id="d2f18-106">Sign-ins that are interactive in nature (where a username/password is passed as part of auth token) and successful federated sign-ins are currently included in the sign-in logs.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2f18-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2f18-107">Permissions</span></span>

<span data-ttu-id="d2f18-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="d2f18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="d2f18-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2f18-110">Permission type</span></span>      | <span data-ttu-id="d2f18-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2f18-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2f18-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2f18-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d2f18-113">AuditLog.Read.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2f18-113">AuditLog.Read.All and Directory.Read.All</span></span> |
|<span data-ttu-id="d2f18-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2f18-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2f18-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d2f18-115">Not supported</span></span>   |
|<span data-ttu-id="d2f18-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d2f18-116">Application</span></span> | <span data-ttu-id="d2f18-117">AuditLog.Read.All и Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2f18-117">AuditLog.Read.All and Directory.Read.All</span></span> |

<span data-ttu-id="d2f18-118">Приложения должны быть [правильно зарегистрированы в](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d2f18-118">Apps must be [properly registered](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to Azure AD.</span></span>

<span data-ttu-id="d2f18-119">Помимо делегирования разрешений, пользователю, входиму в который, необходимо принадлежать к одной из следующих ролей каталога, которая позволяет ему читать отчеты о входе.</span><span class="sxs-lookup"><span data-stu-id="d2f18-119">In addition to the delegated permissions, the signed-in user needs to belong to one of the following directory roles that allow them to read sign-in reports.</span></span> <span data-ttu-id="d2f18-120">Дополнительные информацию о роли каталогов см. в встроенной роли [Azure AD:](/azure/active-directory/roles/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="d2f18-120">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="d2f18-121">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d2f18-121">Global Administrator</span></span>
+ <span data-ttu-id="d2f18-122">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="d2f18-122">Global Reader</span></span>
+ <span data-ttu-id="d2f18-123">Читатель отчетов</span><span class="sxs-lookup"><span data-stu-id="d2f18-123">Reports Reader</span></span>
+ <span data-ttu-id="d2f18-124">"Администратор безопасности"</span><span class="sxs-lookup"><span data-stu-id="d2f18-124">Security Administrator</span></span>
+ <span data-ttu-id="d2f18-125">Оператор безопасности</span><span class="sxs-lookup"><span data-stu-id="d2f18-125">Security Operator</span></span>
+ <span data-ttu-id="d2f18-126">Читатель сведений о безопасности</span><span class="sxs-lookup"><span data-stu-id="d2f18-126">Security Reader</span></span>

## <a name="http-request"></a><span data-ttu-id="d2f18-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2f18-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2f18-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d2f18-128">Optional query parameters</span></span>

<span data-ttu-id="d2f18-129">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d2f18-129">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="d2f18-130">Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="d2f18-130">For details about how to use these parameters, see [OData query parameters](/graph/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2f18-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2f18-131">Request headers</span></span>

| <span data-ttu-id="d2f18-132">Имя</span><span class="sxs-lookup"><span data-stu-id="d2f18-132">Name</span></span>      |<span data-ttu-id="d2f18-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d2f18-133">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d2f18-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2f18-134">Authorization</span></span>  | <span data-ttu-id="d2f18-135">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d2f18-135">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2f18-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2f18-136">Request body</span></span>

<span data-ttu-id="d2f18-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2f18-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2f18-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2f18-138">Response</span></span>

<span data-ttu-id="d2f18-139">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [signIn](../resources/signin.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2f18-139">If successful, this method returns a `200 OK` response code and [signIn](../resources/signin.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2f18-140">Пример</span><span class="sxs-lookup"><span data-stu-id="d2f18-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2f18-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2f18-141">Request</span></span>

<span data-ttu-id="d2f18-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2f18-142">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d2f18-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2f18-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/signIns/66ea54eb-6301-4ee5-be62-ff5a759b0100
```
# <a name="c"></a>[<span data-ttu-id="d2f18-144">C#</span><span class="sxs-lookup"><span data-stu-id="d2f18-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2f18-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2f18-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2f18-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2f18-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2f18-147">Java</span><span class="sxs-lookup"><span data-stu-id="d2f18-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d2f18-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2f18-148">Response</span></span>

<span data-ttu-id="d2f18-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2f18-149">Here is an example of the response.</span></span>
><span data-ttu-id="d2f18-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d2f18-150">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditLogs/signIns",
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

