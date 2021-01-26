---
title: Список governanceRoleSettings
description: Извлечение коллекции governanceRoleSettings для ресурса.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: e4469debdaaa2d6d18fdef6630f3987ba4b2bbab
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981349"
---
# <a name="list-governancerolesettings"></a><span data-ttu-id="2685e-103">Список governanceRoleSettings</span><span class="sxs-lookup"><span data-stu-id="2685e-103">List governanceRoleSettings</span></span>

<span data-ttu-id="2685e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2685e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2685e-105">Извлечение коллекции [governanceRoleSettings для](../resources/governancerolesetting.md) ресурса.</span><span class="sxs-lookup"><span data-stu-id="2685e-105">Retrieve a collection of [governanceRoleSettings](../resources/governancerolesetting.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="2685e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2685e-106">Permissions</span></span>
<span data-ttu-id="2685e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="2685e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="2685e-109">Ресурсы Azure</span><span class="sxs-lookup"><span data-stu-id="2685e-109">Azure resources</span></span>

| <span data-ttu-id="2685e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2685e-110">Permission type</span></span> | <span data-ttu-id="2685e-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2685e-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="2685e-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2685e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2685e-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="2685e-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="2685e-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2685e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2685e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2685e-115">Not supported.</span></span> |
| <span data-ttu-id="2685e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2685e-116">Application</span></span> | <span data-ttu-id="2685e-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="2685e-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="2685e-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="2685e-118">Azure AD</span></span>

| <span data-ttu-id="2685e-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2685e-119">Permission type</span></span> | <span data-ttu-id="2685e-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2685e-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="2685e-121">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2685e-121">Delegated (work or school account)</span></span> | <span data-ttu-id="2685e-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="2685e-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="2685e-123">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2685e-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2685e-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2685e-124">Not supported.</span></span> |
| <span data-ttu-id="2685e-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="2685e-125">Application</span></span> | <span data-ttu-id="2685e-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="2685e-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="2685e-127">Группы</span><span class="sxs-lookup"><span data-stu-id="2685e-127">Groups</span></span>

|<span data-ttu-id="2685e-128">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2685e-128">Permission type</span></span> | <span data-ttu-id="2685e-129">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2685e-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="2685e-130">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2685e-130">Delegated (work or school account)</span></span> | <span data-ttu-id="2685e-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="2685e-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="2685e-132">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2685e-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2685e-133">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2685e-133">Not supported.</span></span> |
| <span data-ttu-id="2685e-134">Приложение</span><span class="sxs-lookup"><span data-stu-id="2685e-134">Application</span></span> | <span data-ttu-id="2685e-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="2685e-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

<span data-ttu-id="2685e-136">Помимо области разрешений, этот API требует, чтобы у запрашивателя было по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="2685e-136">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>
## <a name="http-request"></a><span data-ttu-id="2685e-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2685e-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/<resourceId>/roleSettings
GET /privilegedAccess/azureResources/roleSettings?$filter=resourceId+eq+'<resourceId>'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2685e-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2685e-138">Optional query parameters</span></span>
<span data-ttu-id="2685e-139">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="2685e-139">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2685e-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2685e-140">Request headers</span></span>
| <span data-ttu-id="2685e-141">Имя</span><span class="sxs-lookup"><span data-stu-id="2685e-141">Name</span></span>      |<span data-ttu-id="2685e-142">Описание</span><span class="sxs-lookup"><span data-stu-id="2685e-142">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2685e-143">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2685e-143">Authorization</span></span>  | <span data-ttu-id="2685e-144">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2685e-144">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2685e-145">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2685e-145">Request body</span></span>
<span data-ttu-id="2685e-146">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2685e-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2685e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="2685e-147">Response</span></span>
<span data-ttu-id="2685e-148">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [governanceRoleSetting](../resources/governancerolesetting.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2685e-148">If successful, this method returns a `200 OK` response code and collection of [governanceRoleSetting](../resources/governancerolesetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2685e-149">Пример</span><span class="sxs-lookup"><span data-stu-id="2685e-149">Example</span></span>
<span data-ttu-id="2685e-150">В этом примере показано, как администратор перечисляет параметры роли для ресурса Wingtip Toys - Prod.</span><span class="sxs-lookup"><span data-stu-id="2685e-150">This example shows how an administrator lists role settings for the resource Wingtip Toys - Prod.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_governancerolesettings"
}-->
##### <a name="request"></a><span data-ttu-id="2685e-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="2685e-151">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleSettings
```
##### <a name="response"></a><span data-ttu-id="2685e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="2685e-152">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 463

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleSettings",
    "value": [
        {
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
        },
        {
            "id": "ac642250-9c22-4ec5-a072-02e06c1ef3a0",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "688de08e-66d4-4efe-b234-1cf476a603b9",
            "isDefault": false,
            "lastUpdatedDateTime": "2017-12-07T18:12:43.417Z",
            "lastUpdatedBy": "Allan Deyoung",
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
                    "setting": "{\"Enabled\":true,\"Approvers\":[{\"Id\":\"c178dfee-7236-44b5-a363-e15fc63d91f0\",\"Type\":\"User\",\"DisplayName\":\"Allan Deyoung\",\"Email\":\"AllanD@contoso.com\"}],\"BusinessFlowId\":\"fa7d0b98-ed15-47cd-b3e2-aa6bd3e6533a\"}"
                }
            ]
        },
        ...
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


