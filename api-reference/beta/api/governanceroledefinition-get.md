---
title: Получение Говернанцероледефинитион
description: Получение свойств и связей объекта Говернанцероледефинитион.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 55dbc8933c9adeda1bcd2d40c5ed9c54de7dd55a
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218859"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="6dd96-103">Получение Говернанцероледефинитион</span><span class="sxs-lookup"><span data-stu-id="6dd96-103">Get governanceRoleDefinition</span></span>

<span data-ttu-id="6dd96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dd96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dd96-105">Получение свойств и связей объекта [говернанцероледефинитион](../resources/governanceroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="6dd96-105">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6dd96-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6dd96-106">Permissions</span></span>
<span data-ttu-id="6dd96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dd96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dd96-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dd96-109">Permission type</span></span>      | <span data-ttu-id="6dd96-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6dd96-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dd96-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dd96-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6dd96-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6dd96-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="6dd96-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dd96-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dd96-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dd96-114">Not supported.</span></span>    |
|<span data-ttu-id="6dd96-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6dd96-115">Application</span></span> | <span data-ttu-id="6dd96-116">Привилежедакцесс. Read. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="6dd96-116">PrivilegedAccess.Read.AzureResources</span></span> |

<span data-ttu-id="6dd96-117">Кроме области разрешений, этот API требует, чтобы запрашивающий был иметь по крайней мере одно назначение роли для ресурса, к которому относится [говернанцероледефинитион](../resources/governanceroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="6dd96-117">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="6dd96-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dd96-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6dd96-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6dd96-119">Optional query parameters</span></span>
<span data-ttu-id="6dd96-120">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6dd96-120">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dd96-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6dd96-121">Request headers</span></span>
| <span data-ttu-id="6dd96-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6dd96-122">Name</span></span>      |<span data-ttu-id="6dd96-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6dd96-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6dd96-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6dd96-124">Authorization</span></span>  | <span data-ttu-id="6dd96-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6dd96-125">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="6dd96-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6dd96-126">Request body</span></span>
<span data-ttu-id="6dd96-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6dd96-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6dd96-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="6dd96-128">Response</span></span>
<span data-ttu-id="6dd96-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [говернанцероледефинитион](../resources/governanceroledefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6dd96-129">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6dd96-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6dd96-130">Example</span></span>
<span data-ttu-id="6dd96-131">В этом примере показано, как получить сведения об участниках определения роли DNS в подписке Wingtip Toys-произ.</span><span class="sxs-lookup"><span data-stu-id="6dd96-131">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="6dd96-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dd96-132">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="6dd96-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dd96-133">Response</span></span>
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
  "suppressions": []
}
-->
