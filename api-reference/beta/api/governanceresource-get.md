---
title: Получение governanceResource
description: Извлечение свойств и связи объекта governanceResource.
ms.openlocfilehash: d871dbe91b82cebc01a8c282c0afdfbd8701c8f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075261"
---
# <a name="get-governanceresource"></a><span data-ttu-id="217a3-103">Получение governanceResource</span><span class="sxs-lookup"><span data-stu-id="217a3-103">Get governanceResource</span></span>

> <span data-ttu-id="217a3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="217a3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="217a3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="217a3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="217a3-106">Извлечение свойств и связи объекта [governanceResource](../resources/governanceresource.md) .</span><span class="sxs-lookup"><span data-stu-id="217a3-106">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="217a3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="217a3-107">Permissions</span></span>
<span data-ttu-id="217a3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="217a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="217a3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="217a3-110">Permission type</span></span>      | <span data-ttu-id="217a3-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="217a3-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="217a3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="217a3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="217a3-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="217a3-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="217a3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="217a3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="217a3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="217a3-115">Not supported.</span></span>    |
|<span data-ttu-id="217a3-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="217a3-116">Application</span></span> | <span data-ttu-id="217a3-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="217a3-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="217a3-118">Помимо области разрешений этот интерфейс API требует инициатор запроса может иметь по крайней мере одна роль назначения для ресурса.</span><span class="sxs-lookup"><span data-stu-id="217a3-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="217a3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="217a3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="217a3-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="217a3-120">Optional query parameters</span></span>
<span data-ttu-id="217a3-121">Этот метод **только** поддерживает `$select` и `$expand` [Параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="217a3-121">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="217a3-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="217a3-122">Request headers</span></span>
| <span data-ttu-id="217a3-123">Имя</span><span class="sxs-lookup"><span data-stu-id="217a3-123">Name</span></span>      |<span data-ttu-id="217a3-124">Описание</span><span class="sxs-lookup"><span data-stu-id="217a3-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="217a3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="217a3-125">Authorization</span></span>  | <span data-ttu-id="217a3-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="217a3-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="217a3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="217a3-127">Request body</span></span>
<span data-ttu-id="217a3-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="217a3-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="217a3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="217a3-129">Response</span></span>
<span data-ttu-id="217a3-130">Успешно завершена, этот метод возвращает `200 OK` объект [governanceResource](../resources/governanceresource.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="217a3-130">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="217a3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="217a3-131">Example</span></span>
<span data-ttu-id="217a3-132">В этом примере показано, как получить сведения о подписке Wingtip Toys - производственного (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span><span class="sxs-lookup"><span data-stu-id="217a3-132">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="217a3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="217a3-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="217a3-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="217a3-134">Response</span></span>
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
    "onboardDateTime": "2018-04-05T22:30:37.13Z"
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
