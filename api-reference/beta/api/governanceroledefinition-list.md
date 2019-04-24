---
title: Список Говернанцероледефинитионс
description: Получение коллекции Говернанцероледефинитионс для ресурса.
localization_priority: Normal
ms.openlocfilehash: 0e03a75446723743cc43eef63c42dd0f39c86126
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503067"
---
# <a name="list-governanceroledefinitions"></a><span data-ttu-id="b6c4e-103">Список Говернанцероледефинитионс</span><span class="sxs-lookup"><span data-stu-id="b6c4e-103">List governanceRoleDefinitions</span></span>
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6c4e-104">Получение коллекции [говернанцероледефинитионс](../resources/governanceroledefinition.md) для ресурса.</span><span class="sxs-lookup"><span data-stu-id="b6c4e-104">Get a collection of [governanceRoleDefinitions](../resources/governanceroledefinition.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6c4e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6c4e-105">Permissions</span></span>
<span data-ttu-id="b6c4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6c4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6c4e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b6c4e-108">Permission type</span></span>      | <span data-ttu-id="b6c4e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b6c4e-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6c4e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b6c4e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b6c4e-111">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="b6c4e-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="b6c4e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b6c4e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6c4e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b6c4e-113">Not supported.</span></span>    |
|<span data-ttu-id="b6c4e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b6c4e-114">Application</span></span> | <span data-ttu-id="b6c4e-115">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="b6c4e-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="b6c4e-116">Кроме области разрешений, этот API требует, чтобы запрашивающий был иметь по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="b6c4e-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="b6c4e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b6c4e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions
GET /privilegedAccess/azureResources/roleDefinitions?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b6c4e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b6c4e-118">Optional query parameters</span></span>
<span data-ttu-id="b6c4e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b6c4e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6c4e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b6c4e-120">Request headers</span></span>
| <span data-ttu-id="b6c4e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b6c4e-121">Name</span></span>      |<span data-ttu-id="b6c4e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b6c4e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b6c4e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b6c4e-123">Authorization</span></span>  | <span data-ttu-id="b6c4e-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b6c4e-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6c4e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b6c4e-125">Request body</span></span>
<span data-ttu-id="b6c4e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b6c4e-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b6c4e-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="b6c4e-127">Response</span></span>
<span data-ttu-id="b6c4e-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [говернанцероледефинитион](../resources/governanceroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b6c4e-128">If successful, this method returns a `200 OK` response code and collection of [governanceRoleDefinition](../resources/governanceroledefinition.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b6c4e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b6c4e-129">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinitions"
}-->
<span data-ttu-id="b6c4e-130">В этом примере показано, как получить все определения ролей для группы "компания" Wingtip Toys — произ.</span><span class="sxs-lookup"><span data-stu-id="b6c4e-130">This example shows how to get all role definitions of the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="b6c4e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b6c4e-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions  
```
##### <a name="response"></a><span data-ttu-id="b6c4e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b6c4e-132">Response</span></span>
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
