---
title: Получение Говернанцеролесеттинг
description: Получение свойств и связей объекта Говернанцеролесеттинг.
localization_priority: Normal
ms.openlocfilehash: 2c432c0f680acd2411d57ab6e4b4a7af21f3350a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503097"
---
# <a name="get-governancerolesetting"></a><span data-ttu-id="85f9e-103">Получение Говернанцеролесеттинг</span><span class="sxs-lookup"><span data-stu-id="85f9e-103">Get governanceRoleSetting</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85f9e-104">Получение свойств и связей объекта [говернанцеролесеттинг](../resources/governancerolesetting.md).</span><span class="sxs-lookup"><span data-stu-id="85f9e-104">Retrieve the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="85f9e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85f9e-105">Permissions</span></span>
<span data-ttu-id="85f9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85f9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85f9e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85f9e-108">Permission type</span></span>      | <span data-ttu-id="85f9e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85f9e-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85f9e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85f9e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="85f9e-111">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="85f9e-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="85f9e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85f9e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85f9e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85f9e-113">Not supported.</span></span>    |
|<span data-ttu-id="85f9e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85f9e-114">Application</span></span> | <span data-ttu-id="85f9e-115">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="85f9e-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="85f9e-116">Кроме области разрешений, этот API требует, чтобы запрашивающий был иметь по крайней мере одно назначение роли для ресурса, к которому относится [говернанцеролесеттинг](../resources/governancerolesetting.md) .</span><span class="sxs-lookup"><span data-stu-id="85f9e-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleSetting](../resources/governancerolesetting.md) belongs to.</span></span>
## <a name="http-request"></a><span data-ttu-id="85f9e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85f9e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="85f9e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="85f9e-118">Optional query parameters</span></span>
<span data-ttu-id="85f9e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="85f9e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85f9e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85f9e-120">Request headers</span></span>
| <span data-ttu-id="85f9e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="85f9e-121">Name</span></span>      |<span data-ttu-id="85f9e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="85f9e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="85f9e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85f9e-123">Authorization</span></span>  | <span data-ttu-id="85f9e-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="85f9e-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="85f9e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85f9e-125">Request body</span></span>
<span data-ttu-id="85f9e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85f9e-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="85f9e-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="85f9e-127">Response</span></span>
<span data-ttu-id="85f9e-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [говернанцеролесеттинг](../resources/governancerolesetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85f9e-128">If successful, this method returns a `200 OK` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="85f9e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="85f9e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85f9e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="85f9e-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9
```
##### <a name="response"></a><span data-ttu-id="85f9e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="85f9e-131">Response</span></span>
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
    "Error: /api-reference/beta/api/governancerolesetting-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
