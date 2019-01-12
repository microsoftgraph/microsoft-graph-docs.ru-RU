---
title: Получение identityRiskEvent
description: Извлечение свойств и связи объекта identityriskevent.
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 6b66352010a3f1455dd2598215039c24a2dc819e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935600"
---
# <a name="get-identityriskevent"></a><span data-ttu-id="e296d-103">Получение identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e296d-103">Get identityRiskEvent</span></span>

> <span data-ttu-id="e296d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e296d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e296d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e296d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e296d-106">Извлечение свойств и связи объекта identityriskevent.</span><span class="sxs-lookup"><span data-stu-id="e296d-106">Retrieve the properties and relationships of identityriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e296d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e296d-107">Permissions</span></span>
<span data-ttu-id="e296d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e296d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e296d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e296d-110">Permission type</span></span>      | <span data-ttu-id="e296d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e296d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e296d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e296d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e296d-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e296d-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="e296d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e296d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e296d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e296d-115">Not supported.</span></span>    |
|<span data-ttu-id="e296d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e296d-116">Application</span></span> | <span data-ttu-id="e296d-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e296d-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e296d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e296d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e296d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e296d-119">Request headers</span></span>
| <span data-ttu-id="e296d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e296d-120">Name</span></span>      |<span data-ttu-id="e296d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e296d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e296d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e296d-122">Authorization</span></span>  | <span data-ttu-id="e296d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e296d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e296d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e296d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e296d-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e296d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e296d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e296d-128">Request body</span></span>
<span data-ttu-id="e296d-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e296d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e296d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e296d-130">Response</span></span>

<span data-ttu-id="e296d-131">Успешно завершена, этот метод возвращает `200 OK` объект [identityRiskEvent](../resources/identityriskevent.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e296d-131">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e296d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e296d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e296d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e296d-133">Request</span></span>
<span data-ttu-id="e296d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e296d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```http
GET https://graph.microsoft.com/beta/identityRiskEvents/ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98
```
##### <a name="response"></a><span data-ttu-id="e296d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="e296d-135">Response</span></span>
<span data-ttu-id="e296d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e296d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "c2b6c2b9-dddc-acd0-2b39-d519d803dbc3",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
