---
title: Получение Говернанцероледефинитион
description: Получение свойств и связей объекта Говернанцероледефинитион.
localization_priority: Normal
ms.openlocfilehash: e6a057816a8e07a355941f272325c30078327ab9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503058"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="dd236-103">Получение Говернанцероледефинитион</span><span class="sxs-lookup"><span data-stu-id="dd236-103">Get governanceRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd236-104">Получение свойств и связей объекта [говернанцероледефинитион](../resources/governanceroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="dd236-104">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dd236-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd236-105">Permissions</span></span>
<span data-ttu-id="dd236-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd236-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd236-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd236-108">Permission type</span></span>      | <span data-ttu-id="dd236-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd236-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd236-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd236-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dd236-111">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="dd236-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="dd236-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd236-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd236-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd236-113">Not supported.</span></span>    |
|<span data-ttu-id="dd236-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd236-114">Application</span></span> | <span data-ttu-id="dd236-115">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="dd236-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="dd236-116">Кроме области разрешений, этот API требует, чтобы запрашивающий был иметь по крайней мере одно назначение роли для ресурса, к которому относится [говернанцероледефинитион](../resources/governanceroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="dd236-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="dd236-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd236-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dd236-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dd236-118">Optional query parameters</span></span>
<span data-ttu-id="dd236-119">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="dd236-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd236-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd236-120">Request headers</span></span>
| <span data-ttu-id="dd236-121">Имя</span><span class="sxs-lookup"><span data-stu-id="dd236-121">Name</span></span>      |<span data-ttu-id="dd236-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dd236-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dd236-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd236-123">Authorization</span></span>  | <span data-ttu-id="dd236-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="dd236-124">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="dd236-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd236-125">Request body</span></span>
<span data-ttu-id="dd236-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd236-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="dd236-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="dd236-127">Response</span></span>
<span data-ttu-id="dd236-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [говернанцероледефинитион](../resources/governanceroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd236-128">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dd236-129">Пример</span><span class="sxs-lookup"><span data-stu-id="dd236-129">Example</span></span>
<span data-ttu-id="dd236-130">В этом примере показано, как получить сведения об участниках определения роли DNS в подписке Wingtip Toys-произ.</span><span class="sxs-lookup"><span data-stu-id="dd236-130">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="dd236-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd236-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="dd236-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd236-132">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions/$entity",
    "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
    "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
    "displayName": "DNS Zone Contributor"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroledefinition-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
