---
title: Получение governanceResource
description: Извлечение свойств и связи объекта governanceResource.
ms.openlocfilehash: 55fcea026a2816f33ab6064ea5828d3af4526690
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191083"
---
# <a name="get-governanceresource"></a><span data-ttu-id="794ae-103">Получение governanceResource</span><span class="sxs-lookup"><span data-stu-id="794ae-103">Get governanceResource</span></span>

> <span data-ttu-id="794ae-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="794ae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="794ae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="794ae-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="794ae-106">Извлечение свойств и связи объекта [governanceResource](../resources/governanceresource.md) .</span><span class="sxs-lookup"><span data-stu-id="794ae-106">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="794ae-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="794ae-107">Permissions</span></span>
<span data-ttu-id="794ae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="794ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="794ae-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="794ae-110">Permission type</span></span>      | <span data-ttu-id="794ae-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="794ae-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="794ae-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="794ae-112">Delegated (work or school account)</span></span> | <span data-ttu-id="794ae-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="794ae-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="794ae-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="794ae-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="794ae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="794ae-115">Not supported.</span></span>    |
|<span data-ttu-id="794ae-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="794ae-116">Application</span></span> | <span data-ttu-id="794ae-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="794ae-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="794ae-118">Помимо области разрешений этот интерфейс API требует инициатор запроса может иметь по крайней мере одна роль назначения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="794ae-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="794ae-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="794ae-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="794ae-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="794ae-120">Optional query parameters</span></span>
<span data-ttu-id="794ae-121">Этот метод **только** поддерживает `$select` и `$expand` [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="794ae-121">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="794ae-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="794ae-122">Request headers</span></span>
| <span data-ttu-id="794ae-123">Имя</span><span class="sxs-lookup"><span data-stu-id="794ae-123">Name</span></span>      |<span data-ttu-id="794ae-124">Описание</span><span class="sxs-lookup"><span data-stu-id="794ae-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="794ae-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="794ae-125">Authorization</span></span>  | <span data-ttu-id="794ae-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="794ae-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="794ae-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="794ae-127">Request body</span></span>
<span data-ttu-id="794ae-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="794ae-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="794ae-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="794ae-129">Response</span></span>
<span data-ttu-id="794ae-130">Успешно завершена, этот метод возвращает `200 OK` объект [governanceResource](../resources/governanceresource.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="794ae-130">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="794ae-131">Пример</span><span class="sxs-lookup"><span data-stu-id="794ae-131">Example</span></span>
<span data-ttu-id="794ae-132">В этом примере показано, как получить сведения о подписке Wingtip Toys - производственного (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span><span class="sxs-lookup"><span data-stu-id="794ae-132">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="794ae-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="794ae-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="794ae-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="794ae-134">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
