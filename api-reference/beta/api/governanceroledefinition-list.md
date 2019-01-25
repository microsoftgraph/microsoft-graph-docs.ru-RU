---
title: Список governanceRoleDefinitions
description: Получите коллекцию governanceRoleDefinitions для ресурса.
localization_priority: Normal
ms.openlocfilehash: 0e03a75446723743cc43eef63c42dd0f39c86126
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525201"
---
# <a name="list-governanceroledefinitions"></a><span data-ttu-id="72589-103">Список governanceRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="72589-103">List governanceRoleDefinitions</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72589-104">Получите коллекцию [governanceRoleDefinitions](../resources/governanceroledefinition.md) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="72589-104">Get a collection of [governanceRoleDefinitions](../resources/governanceroledefinition.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="72589-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72589-105">Permissions</span></span>
<span data-ttu-id="72589-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72589-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72589-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72589-108">Permission type</span></span>      | <span data-ttu-id="72589-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72589-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72589-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72589-110">Delegated (work or school account)</span></span> | <span data-ttu-id="72589-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="72589-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="72589-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72589-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72589-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72589-113">Not supported.</span></span>    |
|<span data-ttu-id="72589-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72589-114">Application</span></span> | <span data-ttu-id="72589-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="72589-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="72589-116">Помимо области разрешений этот интерфейс API требует инициатор запроса может иметь по крайней мере одна роль назначения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="72589-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="72589-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72589-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions
GET /privilegedAccess/azureResources/roleDefinitions?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="72589-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="72589-118">Optional query parameters</span></span>
<span data-ttu-id="72589-119">Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.</span><span class="sxs-lookup"><span data-stu-id="72589-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="72589-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72589-120">Request headers</span></span>
| <span data-ttu-id="72589-121">Имя</span><span class="sxs-lookup"><span data-stu-id="72589-121">Name</span></span>      |<span data-ttu-id="72589-122">Описание</span><span class="sxs-lookup"><span data-stu-id="72589-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="72589-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="72589-123">Authorization</span></span>  | <span data-ttu-id="72589-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="72589-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="72589-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72589-125">Request body</span></span>
<span data-ttu-id="72589-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72589-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="72589-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="72589-127">Response</span></span>
<span data-ttu-id="72589-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [governanceRoleDefinition](../resources/governanceroledefinition.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="72589-128">If successful, this method returns a `200 OK` response code and collection of [governanceRoleDefinition](../resources/governanceroledefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="72589-129">Пример</span><span class="sxs-lookup"><span data-stu-id="72589-129">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinitions"
}-->
<span data-ttu-id="72589-130">В этом примере показано, как получить все определения ролей Wingtip Toys - производственного подписки.</span><span class="sxs-lookup"><span data-stu-id="72589-130">This example shows how to get all role definitions of the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="72589-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="72589-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions  
```
##### <a name="response"></a><span data-ttu-id="72589-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="72589-132">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleDefinition",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 21906

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions",
    "value": [
        {
            "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
            "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
            "displayName": "DNS Zone Contributor"
        },
        {
            "id": "051f7264-a992-429a-b345-90415af9f917",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/c12c1c16-33a1-487b-954d-41c89c60f349",
            "templateId": "c12c1c16-33a1-487b-954d-41c89c60f349",
            "displayName": "Reader and Data Access"
        },
        {
            "id": "0789c03d-445d-40ab-aed3-d110a98146c7",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/5d28c62d-5b37-4476-8438-e587778df237",
            "templateId": "5d28c62d-5b37-4476-8438-e587778df237",
            "displayName": "New Relic APM Account Contributor"
        },
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceRoleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroledefinition-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
