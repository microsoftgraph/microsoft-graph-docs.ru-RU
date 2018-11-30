---
title: Получение governanceRoleDefinition
description: Извлечение свойств и отношения governanceRoleDefinition.
ms.openlocfilehash: da6f81c57d8070a977482a81f8f2211b85ab0f97
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081418"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="9d769-103">Получение governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9d769-103">Get governanceRoleDefinition</span></span>

> <span data-ttu-id="9d769-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9d769-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d769-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d769-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d769-106">Извлечение свойств и отношения [governanceRoleDefinition](../resources/governanceroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9d769-106">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9d769-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d769-107">Permissions</span></span>
<span data-ttu-id="9d769-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d769-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d769-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d769-110">Permission type</span></span>      | <span data-ttu-id="9d769-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="9d769-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d769-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d769-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9d769-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9d769-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="9d769-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d769-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d769-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d769-115">Not supported.</span></span>    |
|<span data-ttu-id="9d769-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="9d769-116">Application</span></span> | <span data-ttu-id="9d769-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9d769-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="9d769-118">Помимо области разрешений этот интерфейс API требует инициатор запроса может иметь по крайней мере одно назначение роли на ресурс, который принадлежит [governanceRoleDefinition](../resources/governanceroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="9d769-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="9d769-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d769-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9d769-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9d769-120">Optional query parameters</span></span>
<span data-ttu-id="9d769-121">Метод не **поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа** .</span><span class="sxs-lookup"><span data-stu-id="9d769-121">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d769-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d769-122">Request headers</span></span>
| <span data-ttu-id="9d769-123">Имя</span><span class="sxs-lookup"><span data-stu-id="9d769-123">Name</span></span>      |<span data-ttu-id="9d769-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9d769-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9d769-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d769-125">Authorization</span></span>  | <span data-ttu-id="9d769-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9d769-126">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="9d769-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d769-127">Request body</span></span>
<span data-ttu-id="9d769-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d769-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9d769-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d769-129">Response</span></span>
<span data-ttu-id="9d769-130">Успешно завершена, этот метод возвращает `200 OK` объект [governanceRoleDefinition](../resources/governanceroledefinition.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9d769-130">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9d769-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9d769-131">Example</span></span>
<span data-ttu-id="9d769-132">В этом примере показано, как получить сведения о определение роли корреспондента зону DNS в подписке Wingtip Toys - производственного.</span><span class="sxs-lookup"><span data-stu-id="9d769-132">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="9d769-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d769-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="9d769-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d769-134">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
