---
title: Список Говернанцеролесеттингс
description: Получение коллекции Говернанцеролесеттингс для ресурса.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identitiy-platform
ms.openlocfilehash: c3bfe4470fecfea94ac3a0d2f9b3d81040d07507
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639592"
---
# <a name="list-governancerolesettings"></a><span data-ttu-id="aaff9-103">Список Говернанцеролесеттингс</span><span class="sxs-lookup"><span data-stu-id="aaff9-103">List governanceRoleSettings</span></span>

<span data-ttu-id="aaff9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaff9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aaff9-105">Получение коллекции [говернанцеролесеттингс](../resources/governancerolesetting.md) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="aaff9-105">Retrieve a collection of [governanceRoleSettings](../resources/governancerolesetting.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="aaff9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aaff9-106">Permissions</span></span>
<span data-ttu-id="aaff9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaff9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaff9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aaff9-109">Permission type</span></span>      | <span data-ttu-id="aaff9-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="aaff9-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aaff9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aaff9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aaff9-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="aaff9-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="aaff9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aaff9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaff9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaff9-114">Not supported.</span></span>    |
|<span data-ttu-id="aaff9-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="aaff9-115">Application</span></span> | <span data-ttu-id="aaff9-116">Привилежедакцесс. Read. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="aaff9-116">PrivilegedAccess.Read.AzureResources</span></span> |

<span data-ttu-id="aaff9-117">Кроме области разрешений, этот API требует, чтобы запрашивающий был иметь по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="aaff9-117">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>
## <a name="http-request"></a><span data-ttu-id="aaff9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aaff9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/<resourceId>/roleSettings
GET /privilegedAccess/azureResources/roleSettings?$filter=resourceId+eq+'<resourceId>'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aaff9-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aaff9-119">Optional query parameters</span></span>
<span data-ttu-id="aaff9-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="aaff9-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aaff9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aaff9-121">Request headers</span></span>
| <span data-ttu-id="aaff9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="aaff9-122">Name</span></span>      |<span data-ttu-id="aaff9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="aaff9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aaff9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aaff9-124">Authorization</span></span>  | <span data-ttu-id="aaff9-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="aaff9-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaff9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aaff9-126">Request body</span></span>
<span data-ttu-id="aaff9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aaff9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aaff9-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="aaff9-128">Response</span></span>
<span data-ttu-id="aaff9-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [говернанцеролесеттинг](../resources/governancerolesetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aaff9-129">If successful, this method returns a `200 OK` response code and collection of [governanceRoleSetting](../resources/governancerolesetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaff9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="aaff9-130">Example</span></span>
<span data-ttu-id="aaff9-131">В этом примере показано, как администратор Перечисляет параметры роли для ресурса компания Wingtip Toys — произ.</span><span class="sxs-lookup"><span data-stu-id="aaff9-131">This example shows how an administrator lists role settings for the resource Wingtip Toys - Prod.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_governancerolesettings"
}-->
##### <a name="request"></a><span data-ttu-id="aaff9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aaff9-132">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleSettings
```
##### <a name="response"></a><span data-ttu-id="aaff9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaff9-133">Response</span></span>
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
