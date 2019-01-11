---
title: Получение suspiciousIpRiskEvent
description: Извлечение свойств и связи объекта suspiciousipriskevent.
localization_priority: Normal
ms.openlocfilehash: 1e55300c7d7723e26457b0aedde74dc4f5f6ff1f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836864"
---
# <a name="get-suspiciousipriskevent"></a><span data-ttu-id="7bc99-103">Получение suspiciousIpRiskEvent</span><span class="sxs-lookup"><span data-stu-id="7bc99-103">Get suspiciousIpRiskEvent</span></span>

> <span data-ttu-id="7bc99-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7bc99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7bc99-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bc99-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7bc99-106">Извлечение свойств и связи объекта suspiciousipriskevent.</span><span class="sxs-lookup"><span data-stu-id="7bc99-106">Retrieve the properties and relationships of a suspiciousipriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7bc99-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7bc99-107">Permissions</span></span>
<span data-ttu-id="7bc99-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bc99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bc99-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bc99-110">Permission type</span></span>      | <span data-ttu-id="7bc99-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bc99-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bc99-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bc99-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7bc99-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="7bc99-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="7bc99-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bc99-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bc99-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bc99-115">Not supported.</span></span>    |
|<span data-ttu-id="7bc99-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bc99-116">Application</span></span> | <span data-ttu-id="7bc99-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="7bc99-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bc99-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bc99-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /suspiciousIpRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7bc99-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bc99-119">Request headers</span></span>
| <span data-ttu-id="7bc99-120">Имя</span><span class="sxs-lookup"><span data-stu-id="7bc99-120">Name</span></span>      |<span data-ttu-id="7bc99-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7bc99-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7bc99-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bc99-122">Authorization</span></span>  | <span data-ttu-id="7bc99-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bc99-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7bc99-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="7bc99-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="7bc99-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="7bc99-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bc99-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7bc99-128">Request body</span></span>
<span data-ttu-id="7bc99-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7bc99-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bc99-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7bc99-130">Response</span></span>

<span data-ttu-id="7bc99-131">Успешно завершена, этот метод возвращает `200 OK` объект [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7bc99-131">If successful, this method returns a `200 OK` response code and [suspiciousIpRiskEvent](../resources/suspiciousipriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7bc99-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7bc99-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7bc99-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bc99-133">Request</span></span>
<span data-ttu-id="7bc99-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bc99-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_suspiciousipriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/suspiciousIpRiskEvents/02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475
```
##### <a name="response"></a><span data-ttu-id="7bc99-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="7bc99-135">Response</span></span>
<span data-ttu-id="7bc99-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7bc99-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.suspiciousIpRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": null,
  "createdDateTime": "2016-02-03T06:08:35.123512Z",
  "id": "02e8bfd1-5231-1006-01cc-434f84e0859e-97b7301f-bc05-8e2c-fdfa-2004eb66ff70-287e7b9b-1d60-aa96-6ddb-65c81ee31475",
  "ipAddress": "95.31.18.119",
  "location": "Moskva, Russia, RU",
  "riskEventDateTime": "2016-02-03T05:33:49.9516789Z",
  "riskEventStatus": "active",
  "riskLevel": "low",
  "riskType": "SuspiciousIpRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "97b7301f-bc05-8e2c-fdfa-2004eb66ff70",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get suspiciousIpRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
