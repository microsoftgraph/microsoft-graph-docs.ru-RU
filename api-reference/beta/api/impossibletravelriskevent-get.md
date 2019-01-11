---
title: Получение impossibleTravelRiskEvent
description: Извлечение свойств и связи объекта impossibletravelriskevent.
localization_priority: Normal
ms.openlocfilehash: 6f9c6913fe1bdcd5576814f170eb75d51b28da40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843948"
---
# <a name="get-impossibletravelriskevent"></a><span data-ttu-id="e9ef6-103">Получение impossibleTravelRiskEvent</span><span class="sxs-lookup"><span data-stu-id="e9ef6-103">Get impossibleTravelRiskEvent</span></span>

> <span data-ttu-id="e9ef6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e9ef6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9ef6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9ef6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e9ef6-106">Извлечение свойств и связи объекта impossibletravelriskevent.</span><span class="sxs-lookup"><span data-stu-id="e9ef6-106">Retrieve the properties and relationships of an impossibletravelriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e9ef6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9ef6-107">Permissions</span></span>
<span data-ttu-id="e9ef6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9ef6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9ef6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9ef6-110">Permission type</span></span>      | <span data-ttu-id="e9ef6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9ef6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9ef6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9ef6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e9ef6-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9ef6-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="e9ef6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9ef6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9ef6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9ef6-115">Not supported.</span></span>    |
|<span data-ttu-id="e9ef6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9ef6-116">Application</span></span> | <span data-ttu-id="e9ef6-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9ef6-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9ef6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9ef6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /impossibleTravelRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e9ef6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9ef6-119">Request headers</span></span>
| <span data-ttu-id="e9ef6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="e9ef6-120">Name</span></span>      |<span data-ttu-id="e9ef6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e9ef6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e9ef6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9ef6-122">Authorization</span></span>  | <span data-ttu-id="e9ef6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9ef6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e9ef6-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="e9ef6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="e9ef6-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="e9ef6-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9ef6-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9ef6-128">Request body</span></span>
<span data-ttu-id="e9ef6-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e9ef6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9ef6-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9ef6-130">Response</span></span>

<span data-ttu-id="e9ef6-131">Успешно завершена, этот метод возвращает `200 OK` объект [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e9ef6-131">If successful, this method returns a `200 OK` response code and [impossibleTravelRiskEvent](../resources/impossibletravelriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e9ef6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="e9ef6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e9ef6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9ef6-133">Request</span></span>
<span data-ttu-id="e9ef6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9ef6-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_impossibletravelriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/impossibleTravelRiskEvents/22e65c1f-909a-42b5-c0d2-075f30e27887-0bfdc7a8-6a16-c33e-7de9-a60a28ae533b-15475553-dbc1-8879-5079-23b1edd25bab
```
##### <a name="response"></a><span data-ttu-id="e9ef6-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9ef6-135">Response</span></span>
<span data-ttu-id="e9ef6-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e9ef6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 260

{
  "@odata.type": "#microsoft.graph.impossibleTravelRiskEvent",
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "22e65c1f-909a-42b5-c0d2-075f30e27887-0bfdc7a8-6a16-c33e-7de9-a60a28ae533b-15475553-dbc1-8879-5079-23b1edd25bab",
  "ipAddress": "176.10.104.240",
  "isAtypicalLocation": true,
  "location": "Bern, CH",
  "previousIPAddress": "95.31.18.119",
  "previousLocation": "Moskva, Russia, RU",
  "previousSigninDateTime": "2016-01-29T00:00:55.3859274Z",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "ImpossibleTravelRiskEvent",
  "userAgent": "Firefox 42.0.0.1",
  "userDisplayName": "Jon Doe",
  "userId": "0bfdc7a8-6a16-c33e-7de9-a60a28ae533b",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get impossibleTravelRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
