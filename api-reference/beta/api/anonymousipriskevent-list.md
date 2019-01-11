---
title: Список anonymousIpRiskEvents
description: Получение списка объектов anonymousipriskevent.
localization_priority: Normal
ms.openlocfilehash: 83aa906a936d1a33657446f69d512ecd3a0e6e88
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854917"
---
# <a name="list-anonymousipriskevents"></a><span data-ttu-id="cd690-103">Список anonymousIpRiskEvents</span><span class="sxs-lookup"><span data-stu-id="cd690-103">List anonymousIpRiskEvents</span></span>

> <span data-ttu-id="cd690-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cd690-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd690-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd690-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd690-106">Получение списка объектов anonymousipriskevent.</span><span class="sxs-lookup"><span data-stu-id="cd690-106">Retrieve a list of anonymousipriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="cd690-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd690-107">Permissions</span></span>
<span data-ttu-id="cd690-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd690-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd690-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd690-110">Permission type</span></span>      | <span data-ttu-id="cd690-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd690-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd690-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd690-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cd690-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd690-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="cd690-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd690-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd690-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd690-115">Not supported.</span></span>    |
|<span data-ttu-id="cd690-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd690-116">Application</span></span> | <span data-ttu-id="cd690-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd690-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd690-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd690-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents
```

## <a name="request-headers"></a><span data-ttu-id="cd690-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd690-119">Request headers</span></span>
| <span data-ttu-id="cd690-120">Имя</span><span class="sxs-lookup"><span data-stu-id="cd690-120">Name</span></span>      |<span data-ttu-id="cd690-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cd690-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cd690-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd690-122">Authorization</span></span>  | <span data-ttu-id="cd690-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd690-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cd690-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cd690-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="cd690-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="cd690-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd690-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cd690-128">Request body</span></span>
<span data-ttu-id="cd690-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cd690-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd690-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd690-130">Response</span></span>

<span data-ttu-id="cd690-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cd690-131">If successful, this method returns a `200 OK` response code and collection of [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cd690-132">Пример</span><span class="sxs-lookup"><span data-stu-id="cd690-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd690-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd690-133">Request</span></span>
<span data-ttu-id="cd690-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd690-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents
```
##### <a name="response"></a><span data-ttu-id="cd690-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd690-135">Response</span></span>
<span data-ttu-id="cd690-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cd690-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 290

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List anonymousIpRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
