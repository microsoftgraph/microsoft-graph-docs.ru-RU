---
title: Get governanceRoleSetting
description: Извлечение свойств и связей объекта governanceRoleSetting.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 26fcb5363118f74665a7bf319f8ab65a4df10c50
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983379"
---
# <a name="get-governancerolesetting"></a><span data-ttu-id="15126-103">Get governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="15126-103">Get governanceRoleSetting</span></span>

<span data-ttu-id="15126-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15126-104">Namespace: microsoft.graph</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15126-105">Извлечение свойств и связей [объекта governanceRoleSetting.](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="15126-105">Retrieve the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="15126-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15126-106">Permissions</span></span>
<span data-ttu-id="15126-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="15126-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="15126-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="15126-109">Azure resources</span></span>

| <span data-ttu-id="15126-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15126-110">Permission type</span></span> | <span data-ttu-id="15126-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15126-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="15126-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15126-112">Delegated (work or school account)</span></span> | <span data-ttu-id="15126-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="15126-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="15126-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15126-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15126-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15126-115">Not supported.</span></span> |
| <span data-ttu-id="15126-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="15126-116">Application</span></span> | <span data-ttu-id="15126-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="15126-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="15126-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="15126-118">Azure AD</span></span>

| <span data-ttu-id="15126-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15126-119">Permission type</span></span> | <span data-ttu-id="15126-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15126-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="15126-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15126-121">Delegated (work or school account)</span></span> | <span data-ttu-id="15126-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="15126-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="15126-123">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15126-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15126-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15126-124">Not supported.</span></span> |
| <span data-ttu-id="15126-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="15126-125">Application</span></span> | <span data-ttu-id="15126-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="15126-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="15126-127">Группы</span><span class="sxs-lookup"><span data-stu-id="15126-127">Groups</span></span>

|<span data-ttu-id="15126-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15126-128">Permission type</span></span> | <span data-ttu-id="15126-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15126-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="15126-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15126-130">Delegated (work or school account)</span></span> | <span data-ttu-id="15126-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="15126-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="15126-132">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15126-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15126-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15126-133">Not supported.</span></span> |
| <span data-ttu-id="15126-134">Приложение</span><span class="sxs-lookup"><span data-stu-id="15126-134">Application</span></span> | <span data-ttu-id="15126-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="15126-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="15126-136">Помимо области разрешений, этот API требует, чтобы у запрашивателя было по крайней мере одно назначение роли для ресурса, которому принадлежит [governanceRoleSetting.](../resources/governancerolesetting.md)</span><span class="sxs-lookup"><span data-stu-id="15126-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleSetting](../resources/governancerolesetting.md) belongs to.</span></span>
## <a name="http-request"></a><span data-ttu-id="15126-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15126-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="15126-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="15126-138">Optional query parameters</span></span>
<span data-ttu-id="15126-139">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="15126-139">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15126-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15126-140">Request headers</span></span>
| <span data-ttu-id="15126-141">Имя</span><span class="sxs-lookup"><span data-stu-id="15126-141">Name</span></span>      |<span data-ttu-id="15126-142">Описание</span><span class="sxs-lookup"><span data-stu-id="15126-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="15126-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15126-143">Authorization</span></span>  | <span data-ttu-id="15126-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="15126-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="15126-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15126-145">Request body</span></span>
<span data-ttu-id="15126-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="15126-146">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="15126-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="15126-147">Response</span></span>
<span data-ttu-id="15126-148">В случае успеха этот метод возвращает код отклика и объект `200 OK` [governanceRoleSetting](../resources/governancerolesetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15126-148">If successful, this method returns a `200 OK` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="15126-149">Пример</span><span class="sxs-lookup"><span data-stu-id="15126-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="15126-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="15126-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="15126-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="15126-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9
```
# <a name="c"></a>[<span data-ttu-id="15126-152">C#</span><span class="sxs-lookup"><span data-stu-id="15126-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="15126-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15126-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15126-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15126-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="15126-155">Java</span><span class="sxs-lookup"><span data-stu-id="15126-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-governancerolesetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="15126-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="15126-156">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 370

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleSettings/$entity",
    "id": "80dc5d6f-8d89-47b3-953f-01dc909ed3f9",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "5b8bea96-e9f6-4c63-a8e9-fb092c79f0a1",
    "isDefault": false,
    "lastUpdatedDateTime": "2018-03-26T21:21:43.113Z",
    "lastUpdatedBy": "Alex Wilber",
    "adminEligibleSettings": [
        {
            "ruleIdentifier": "ExpirationRule",
            "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
        }
    ],
    "adminMemberSettings": [
        {
            "ruleIdentifier": "ExpirationRule",
            "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":43200}"
        },
        {
            "ruleIdentifier": "MfaRule",
            "setting": "{\"mfaRequired\":false}"
        },
        {
            "ruleIdentifier": "JustificationRule",
            "setting": "{\"required\":true}"
        }
    ],
    "userEligibleSettings": [],
    "userMemberSettings": [
        {
            "ruleIdentifier": "ExpirationRule",
            "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":480}"
        },
        {
            "ruleIdentifier": "MfaRule",
            "setting": "{\"mfaRequired\":false}"
        },
        {
            "ruleIdentifier": "JustificationRule",
            "setting": "{\"required\":true}"
        },
        {
            "ruleIdentifier": "ApprovalRule",
            "setting": "{\"Enabled\":true,\"Approvers\":[{\"Id\":\"20083cf1-b8d8-43be-9d37-96adfb09e619\",\"Type\":\"User\",\"DisplayName\":\"Alex Wilber\",\"Email\":\"AlexW@contoso.com\"},{\"Id\":\"d158e1b0-5080-4088-a1e7-9ca54f39eb53\",\"Type\":\"User\",\"DisplayName\":\"Alex Wilber\",\"Email\":\"AlexW@contoso.com\"}],\"BusinessFlowId\":\"8df9e93a-6ba9-4453-af43-07cb95435032\"}"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


