---
title: Получение Говернанцеролесеттинг
description: Получение свойств и связей объекта Говернанцеролесеттинг.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identitiy-platform
ms.openlocfilehash: dbe1540541fb21d023fc644682d390652f5f5707
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639620"
---
# <a name="get-governancerolesetting"></a><span data-ttu-id="5966b-103">Получение Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="5966b-103">Get governanceRoleSetting</span></span>

<span data-ttu-id="5966b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5966b-104">Namespace: microsoft.graph</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5966b-105">Получение свойств и связей объекта [говернанцеролесеттинг](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="5966b-105">Retrieve the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5966b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5966b-106">Permissions</span></span>
<span data-ttu-id="5966b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5966b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5966b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5966b-109">Permission type</span></span>      | <span data-ttu-id="5966b-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="5966b-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5966b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5966b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5966b-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="5966b-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="5966b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5966b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5966b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5966b-114">Not supported.</span></span>    |
|<span data-ttu-id="5966b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="5966b-115">Application</span></span> | <span data-ttu-id="5966b-116">Привилежедакцесс. Read. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="5966b-116">PrivilegedAccess.Read.AzureResources</span></span> |

<span data-ttu-id="5966b-117">Кроме области разрешений, этот API требует, чтобы запрашивающий был иметь по крайней мере одно назначение роли для ресурса, к которому относится [говернанцеролесеттинг](../resources/governancerolesetting.md) .</span><span class="sxs-lookup"><span data-stu-id="5966b-117">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleSetting](../resources/governancerolesetting.md) belongs to.</span></span>
## <a name="http-request"></a><span data-ttu-id="5966b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5966b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5966b-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5966b-119">Optional query parameters</span></span>
<span data-ttu-id="5966b-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5966b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5966b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5966b-121">Request headers</span></span>
| <span data-ttu-id="5966b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5966b-122">Name</span></span>      |<span data-ttu-id="5966b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="5966b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5966b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5966b-124">Authorization</span></span>  | <span data-ttu-id="5966b-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5966b-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5966b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5966b-126">Request body</span></span>
<span data-ttu-id="5966b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5966b-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5966b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="5966b-128">Response</span></span>
<span data-ttu-id="5966b-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [говернанцеролесеттинг](../resources/governancerolesetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5966b-129">If successful, this method returns a `200 OK` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5966b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5966b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5966b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5966b-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5966b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5966b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9
```
# <a name="c"></a>[<span data-ttu-id="5966b-133">C#</span><span class="sxs-lookup"><span data-stu-id="5966b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5966b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5966b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5966b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5966b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5966b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5966b-136">Response</span></span>
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
