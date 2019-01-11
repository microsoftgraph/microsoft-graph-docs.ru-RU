---
title: Получение anonymousIpRiskEvent
description: Извлечение свойств и связи объекта anonymousipriskevent.
localization_priority: Normal
ms.openlocfilehash: a4a1483dd3b4bc984a418f1ff03083bf2977b5a4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859929"
---
# <a name="get-anonymousipriskevent"></a><span data-ttu-id="76e0b-103">Получение anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="76e0b-103">Get anonymousIpRiskEvent</span></span>

> <span data-ttu-id="76e0b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="76e0b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76e0b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76e0b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76e0b-106">Извлечение свойств и связи объекта anonymousipriskevent.</span><span class="sxs-lookup"><span data-stu-id="76e0b-106">Retrieve the properties and relationships of an anonymousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="76e0b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76e0b-107">Permissions</span></span>
<span data-ttu-id="76e0b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76e0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76e0b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76e0b-110">Permission type</span></span>      | <span data-ttu-id="76e0b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76e0b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76e0b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76e0b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="76e0b-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="76e0b-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="76e0b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76e0b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76e0b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76e0b-115">Not supported.</span></span>    |
|<span data-ttu-id="76e0b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76e0b-116">Application</span></span> | <span data-ttu-id="76e0b-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="76e0b-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76e0b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76e0b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="76e0b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76e0b-119">Request headers</span></span>
| <span data-ttu-id="76e0b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="76e0b-120">Name</span></span>      |<span data-ttu-id="76e0b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="76e0b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="76e0b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76e0b-122">Authorization</span></span>  | <span data-ttu-id="76e0b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76e0b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76e0b-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="76e0b-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="76e0b-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="76e0b-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="76e0b-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="76e0b-128">Request body</span></span>
<span data-ttu-id="76e0b-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="76e0b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76e0b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="76e0b-130">Response</span></span>

<span data-ttu-id="76e0b-131">Успешно завершена, этот метод возвращает `200 OK` объект [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) и кода ответа в значении тело ответа.</span><span class="sxs-lookup"><span data-stu-id="76e0b-131">If successful, this method returns a `200 OK` response code and [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object in the value of response body.</span></span>
## <a name="example"></a><span data-ttu-id="76e0b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="76e0b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76e0b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="76e0b-133">Request</span></span>
<span data-ttu-id="76e0b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76e0b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents/2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71
```
##### <a name="response"></a><span data-ttu-id="76e0b-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="76e0b-135">Response</span></span>
<span data-ttu-id="76e0b-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="76e0b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71",
  "ipAddress": null,
  "location": null,
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "AnonymousIpRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "6a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get anonymousIpRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
