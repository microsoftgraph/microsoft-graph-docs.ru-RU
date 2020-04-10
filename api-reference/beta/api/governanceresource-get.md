---
title: Получение governanceResource
description: Получение свойств и связей объекта governanceResource.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: cc9eb38838ce4dbbd06888cb4b5d004e7ee6e150
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218929"
---
# <a name="get-governanceresource"></a><span data-ttu-id="94a7a-103">Получение governanceResource</span><span class="sxs-lookup"><span data-stu-id="94a7a-103">Get governanceResource</span></span>

<span data-ttu-id="94a7a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94a7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94a7a-105">Получение свойств и связей объекта [governanceResource](../resources/governanceresource.md) .</span><span class="sxs-lookup"><span data-stu-id="94a7a-105">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="94a7a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94a7a-106">Permissions</span></span>
<span data-ttu-id="94a7a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94a7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94a7a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94a7a-109">Permission type</span></span>      | <span data-ttu-id="94a7a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94a7a-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94a7a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94a7a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="94a7a-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="94a7a-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="94a7a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94a7a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94a7a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94a7a-114">Not supported.</span></span>    |
|<span data-ttu-id="94a7a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94a7a-115">Application</span></span> | <span data-ttu-id="94a7a-116">Привилежедакцесс. Read. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="94a7a-116">PrivilegedAccess.Read.AzureResources</span></span> |

<span data-ttu-id="94a7a-117">Кроме области разрешений, этот API требует, чтобы запрашивающий был иметь по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="94a7a-117">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="94a7a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94a7a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94a7a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="94a7a-119">Optional query parameters</span></span>
<span data-ttu-id="94a7a-120">Этот метод **only** поддерживает `$select` `$expand` только [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="94a7a-120">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94a7a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94a7a-121">Request headers</span></span>
| <span data-ttu-id="94a7a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="94a7a-122">Name</span></span>      |<span data-ttu-id="94a7a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="94a7a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94a7a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94a7a-124">Authorization</span></span>  | <span data-ttu-id="94a7a-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="94a7a-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="94a7a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94a7a-126">Request body</span></span>
<span data-ttu-id="94a7a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94a7a-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="94a7a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="94a7a-128">Response</span></span>
<span data-ttu-id="94a7a-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [governanceResource](../resources/governanceresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="94a7a-129">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94a7a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="94a7a-130">Example</span></span>
<span data-ttu-id="94a7a-131">В этом примере показано, как получить сведения о подписке Wingtip Toys-произ (e5e7d29d-5465-45AC-885f-4716a5ee74b5).</span><span class="sxs-lookup"><span data-stu-id="94a7a-131">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="94a7a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="94a7a-132">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="94a7a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="94a7a-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 459

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources/$entity",
    "id": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",
    "type": "subscription",
    "displayName": "Wingtip Toys - Prod",
    "status": "Active",
    "registeredDateTime": "2018-04-05T22:30:37.13Z",
    "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
