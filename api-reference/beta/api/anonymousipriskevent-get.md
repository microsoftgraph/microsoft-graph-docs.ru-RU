---
title: Получение anonymousIpRiskEvent
description: Извлечение свойств и связи объекта anonymousipriskevent.
ms.openlocfilehash: 0dbc53f53ed029939cc02454041b63e6360d83c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076317"
---
# <a name="get-anonymousipriskevent"></a><span data-ttu-id="6d14d-103">Получение anonymousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="6d14d-103">Get anonymousIpRiskEvent</span></span>

> <span data-ttu-id="6d14d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6d14d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d14d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d14d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6d14d-106">Извлечение свойств и связи объекта anonymousipriskevent.</span><span class="sxs-lookup"><span data-stu-id="6d14d-106">Retrieve the properties and relationships of an anonymousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6d14d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d14d-107">Permissions</span></span>
<span data-ttu-id="6d14d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d14d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d14d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d14d-110">Permission type</span></span>      | <span data-ttu-id="6d14d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d14d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d14d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d14d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6d14d-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d14d-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="6d14d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d14d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d14d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d14d-115">Not supported.</span></span>    |
|<span data-ttu-id="6d14d-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="6d14d-116">Application</span></span> | <span data-ttu-id="6d14d-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d14d-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d14d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d14d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6d14d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d14d-119">Request headers</span></span>
| <span data-ttu-id="6d14d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6d14d-120">Name</span></span>      |<span data-ttu-id="6d14d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6d14d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6d14d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d14d-122">Authorization</span></span>  | <span data-ttu-id="6d14d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d14d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6d14d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="6d14d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="6d14d-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="6d14d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d14d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d14d-128">Request body</span></span>
<span data-ttu-id="6d14d-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d14d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d14d-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d14d-130">Response</span></span>

<span data-ttu-id="6d14d-131">Успешно завершена, этот метод возвращает `200 OK` объект [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) и кода ответа в значении тело ответа.</span><span class="sxs-lookup"><span data-stu-id="6d14d-131">If successful, this method returns a `200 OK` response code and [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) object in the value of response body.</span></span>
## <a name="example"></a><span data-ttu-id="6d14d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6d14d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d14d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d14d-133">Request</span></span>
<span data-ttu-id="6d14d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d14d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents/2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71
```
##### <a name="response"></a><span data-ttu-id="6d14d-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="6d14d-135">Response</span></span>
<span data-ttu-id="6d14d-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6d14d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
