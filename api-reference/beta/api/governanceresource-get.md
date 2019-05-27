---
title: Получение governanceResource
description: Получение свойств и связей объекта governanceResource.
localization_priority: Normal
ms.openlocfilehash: 346ebe770b12d9a66c77951521e59b453fbc8ea6
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422432"
---
# <a name="get-governanceresource"></a><span data-ttu-id="494de-103">Получение governanceResource</span><span class="sxs-lookup"><span data-stu-id="494de-103">Get governanceResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="494de-104">Получение свойств и связей объекта [governanceResource](../resources/governanceresource.md) .</span><span class="sxs-lookup"><span data-stu-id="494de-104">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="494de-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="494de-105">Permissions</span></span>
<span data-ttu-id="494de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="494de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="494de-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="494de-108">Permission type</span></span>      | <span data-ttu-id="494de-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="494de-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="494de-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="494de-110">Delegated (work or school account)</span></span> | <span data-ttu-id="494de-111">Привилежедакцесс. ReadWrite. Азурересаурцес</span><span class="sxs-lookup"><span data-stu-id="494de-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="494de-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="494de-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="494de-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="494de-113">Not supported.</span></span>    |
|<span data-ttu-id="494de-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="494de-114">Application</span></span> | <span data-ttu-id="494de-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="494de-115">Not supported.</span></span> |

<span data-ttu-id="494de-116">Кроме области разрешений, этот API требует, чтобы запрашивающий был иметь по крайней мере одно назначение роли для ресурса.</span><span class="sxs-lookup"><span data-stu-id="494de-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="494de-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="494de-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="494de-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="494de-118">Optional query parameters</span></span>
<span data-ttu-id="494de-119">Этот метод \*\*\*\* поддерживает `$select` `$expand` только [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="494de-119">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="494de-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="494de-120">Request headers</span></span>
| <span data-ttu-id="494de-121">Имя</span><span class="sxs-lookup"><span data-stu-id="494de-121">Name</span></span>      |<span data-ttu-id="494de-122">Описание</span><span class="sxs-lookup"><span data-stu-id="494de-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="494de-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="494de-123">Authorization</span></span>  | <span data-ttu-id="494de-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="494de-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="494de-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="494de-125">Request body</span></span>
<span data-ttu-id="494de-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="494de-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="494de-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="494de-127">Response</span></span>
<span data-ttu-id="494de-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [governanceResource](../resources/governanceresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="494de-128">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="494de-129">Пример</span><span class="sxs-lookup"><span data-stu-id="494de-129">Example</span></span>
<span data-ttu-id="494de-130">В этом примере показано, как получить сведения о подписке Wingtip Toys-произ (e5e7d29d-5465-45AC-885f-4716a5ee74b5).</span><span class="sxs-lookup"><span data-stu-id="494de-130">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="494de-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="494de-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="494de-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="494de-132">Response</span></span>
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
