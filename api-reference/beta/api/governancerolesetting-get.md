---
title: Получение governanceRoleSetting
description: Извлечение свойств и отношения governanceRoleSetting.
localization_priority: Normal
ms.openlocfilehash: db4c2a287ba1089c4aac73b9f0cf6e204a726c86
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864514"
---
# <a name="get-governancerolesetting"></a><span data-ttu-id="effba-103">Получение governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="effba-103">Get governanceRoleSetting</span></span>


> <span data-ttu-id="effba-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="effba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="effba-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="effba-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="effba-106">Извлечение свойств и отношения [governanceRoleSetting](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="effba-106">Retrieve the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="effba-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="effba-107">Permissions</span></span>
<span data-ttu-id="effba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="effba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="effba-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="effba-110">Permission type</span></span>      | <span data-ttu-id="effba-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="effba-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="effba-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="effba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="effba-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="effba-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="effba-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="effba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="effba-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="effba-115">Not supported.</span></span>    |
|<span data-ttu-id="effba-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="effba-116">Application</span></span> | <span data-ttu-id="effba-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="effba-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="effba-118">Помимо области разрешений этот интерфейс API требует инициатор запроса может иметь по крайней мере одно назначение роли на ресурс, который принадлежит [governanceRoleSetting](../resources/governancerolesetting.md) .</span><span class="sxs-lookup"><span data-stu-id="effba-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleSetting](../resources/governancerolesetting.md) belongs to.</span></span>
## <a name="http-request"></a><span data-ttu-id="effba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="effba-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="effba-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="effba-120">Optional query parameters</span></span>
<span data-ttu-id="effba-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="effba-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="effba-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="effba-122">Request headers</span></span>
| <span data-ttu-id="effba-123">Имя</span><span class="sxs-lookup"><span data-stu-id="effba-123">Name</span></span>      |<span data-ttu-id="effba-124">Описание</span><span class="sxs-lookup"><span data-stu-id="effba-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="effba-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="effba-125">Authorization</span></span>  | <span data-ttu-id="effba-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="effba-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="effba-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="effba-127">Request body</span></span>
<span data-ttu-id="effba-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="effba-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="effba-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="effba-129">Response</span></span>
<span data-ttu-id="effba-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [governanceRoleSetting](../resources/governancerolesetting.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="effba-130">If successful, this method returns a `200 OK` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="effba-131">Пример</span><span class="sxs-lookup"><span data-stu-id="effba-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="effba-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="effba-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9
```
##### <a name="response"></a><span data-ttu-id="effba-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="effba-133">Response</span></span>
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
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
