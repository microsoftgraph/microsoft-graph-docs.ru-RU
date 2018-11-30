---
title: Список governanceRoleSettings
description: Получите коллекцию governanceRoleSettings для ресурса.
ms.openlocfilehash: 81aa141cecdfce65f8ca2934b2464f5978b96eac
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075605"
---
# <a name="list-governancerolesettings"></a><span data-ttu-id="3a965-103">Список governanceRoleSettings</span><span class="sxs-lookup"><span data-stu-id="3a965-103">List governanceRoleSettings</span></span>

> <span data-ttu-id="3a965-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3a965-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a965-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a965-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a965-106">Получите коллекцию [governanceRoleSettings](../resources/governancerolesetting.md) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="3a965-106">Retrieve a collection of [governanceRoleSettings](../resources/governancerolesetting.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a965-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a965-107">Permissions</span></span>
<span data-ttu-id="3a965-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a965-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a965-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a965-110">Permission type</span></span>      | <span data-ttu-id="3a965-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="3a965-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a965-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a965-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3a965-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="3a965-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="3a965-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a965-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a965-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a965-115">Not supported.</span></span>    |
|<span data-ttu-id="3a965-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="3a965-116">Application</span></span> | <span data-ttu-id="3a965-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="3a965-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="3a965-118">Помимо области разрешений этот интерфейс API требует инициатор запроса может иметь по крайней мере одна роль назначения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="3a965-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>
## <a name="http-request"></a><span data-ttu-id="3a965-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a965-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/<resourceId>/roleSettings
GET /privilegedAccess/azureResources/roleSettings?$filter=resourceId+eq+'<resourceId>'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3a965-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3a965-120">Optional query parameters</span></span>
<span data-ttu-id="3a965-121">Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="3a965-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a965-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a965-122">Request headers</span></span>
| <span data-ttu-id="3a965-123">Имя</span><span class="sxs-lookup"><span data-stu-id="3a965-123">Name</span></span>      |<span data-ttu-id="3a965-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3a965-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3a965-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a965-125">Authorization</span></span>  | <span data-ttu-id="3a965-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3a965-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a965-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a965-127">Request body</span></span>
<span data-ttu-id="3a965-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a965-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a965-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a965-129">Response</span></span>
<span data-ttu-id="3a965-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [governanceRoleSetting](../resources/governancerolesetting.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3a965-130">If successful, this method returns a `200 OK` response code and collection of [governanceRoleSetting](../resources/governancerolesetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a965-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3a965-131">Example</span></span>
<span data-ttu-id="3a965-132">В этом примере показано, как администратор перечислены параметры ролей для ресурса Wingtip Toys - производственного.</span><span class="sxs-lookup"><span data-stu-id="3a965-132">This example shows how an administrator lists role settings for the resource Wingtip Toys - Prod.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_governancerolesettings"
}-->
##### <a name="request"></a><span data-ttu-id="3a965-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a965-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleSettings
```
##### <a name="response"></a><span data-ttu-id="3a965-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a965-134">Response</span></span>
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
            "lastUpdatedBy": "Vishal Seri",
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
                    "setting": "{\"Enabled\":true,\"Approvers\":[{\"Id\":\"20083cf1-b8d8-43be-9d37-96adfb09e619\",\"Type\":\"User\",\"DisplayName\":\"Vishal Seri\",\"Email\":\"viseri@fimdev.net\"},{\"Id\":\"d158e1b0-5080-4088-a1e7-9ca54f39eb53\",\"Type\":\"User\",\"DisplayName\":\"viseri\",\"Email\":\"viseri@microsoft.com\"}],\"BusinessFlowId\":\"8df9e93a-6ba9-4453-af43-07cb95435032\"}"
                }
            ]
        },
        {
            "id": "ac642250-9c22-4ec5-a072-02e06c1ef3a0",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "688de08e-66d4-4efe-b234-1cf476a603b9",
            "isDefault": false,
            "lastUpdatedDateTime": "2017-12-07T18:12:43.417Z",
            "lastUpdatedBy": "Debashis Choudhury",
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
                    "setting": "{\"Enabled\":true,\"Approvers\":[{\"Id\":\"c178dfee-7236-44b5-a363-e15fc63d91f0\",\"Type\":\"User\",\"DisplayName\":\"Debashis Choudhury\",\"Email\":\"debac@fimdev.net\"}],\"BusinessFlowId\":\"fa7d0b98-ed15-47cd-b3e2-aa6bd3e6533a\"}"
                }
            ]
        },
        ...
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List governanceRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
