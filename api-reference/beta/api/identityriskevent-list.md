---
title: Список identityRiskEvents
description: Получение списка объектов identityriskevent.
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 928c7e548a43bbb62958ae03d03e747adff8a397
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941235"
---
# <a name="list-identityriskevents"></a><span data-ttu-id="30226-103">Список identityRiskEvents</span><span class="sxs-lookup"><span data-stu-id="30226-103">List identityRiskEvents</span></span>

> <span data-ttu-id="30226-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="30226-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30226-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30226-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="30226-106">Получение списка объектов identityriskevent.</span><span class="sxs-lookup"><span data-stu-id="30226-106">Retrieve a list of identityriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="30226-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30226-107">Permissions</span></span>
<span data-ttu-id="30226-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30226-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30226-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30226-110">Permission type</span></span>      | <span data-ttu-id="30226-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30226-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30226-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30226-112">Delegated (work or school account)</span></span> | <span data-ttu-id="30226-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="30226-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="30226-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30226-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30226-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30226-115">Not supported.</span></span>    |
|<span data-ttu-id="30226-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30226-116">Application</span></span> | <span data-ttu-id="30226-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="30226-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="30226-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30226-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="30226-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30226-119">Request headers</span></span>
| <span data-ttu-id="30226-120">Имя</span><span class="sxs-lookup"><span data-stu-id="30226-120">Name</span></span>      |<span data-ttu-id="30226-121">Описание</span><span class="sxs-lookup"><span data-stu-id="30226-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="30226-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30226-122">Authorization</span></span>  | <span data-ttu-id="30226-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30226-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="30226-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="30226-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="30226-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="30226-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="30226-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="30226-128">Request body</span></span>
<span data-ttu-id="30226-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30226-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30226-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="30226-130">Response</span></span>

<span data-ttu-id="30226-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [identityRiskEvent](../resources/identityriskevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="30226-131">If successful, this method returns a `200 OK` response code and collection of [identityRiskEvent](../resources/identityriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="30226-132">Пример</span><span class="sxs-lookup"><span data-stu-id="30226-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30226-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="30226-133">Request</span></span>
<span data-ttu-id="30226-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30226-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityRiskEvents
```
##### <a name="response"></a><span data-ttu-id="30226-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="30226-135">Response</span></span>
<span data-ttu-id="30226-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="30226-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.malwareRiskEvent",
      "malwareName": "CONFICKER",
      "closedDateTime": null,
      "createdDateTime": "2016-02-03T06:06:01.940814Z",
      "deviceInformation": "B62XYZ13OX",
      "id": "74ceb0af-2271-9167-ffa0-b6ac3b4e8781-9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89-0fdc2304-ba4c-ac0c-bdd7-da2d10e93849",
      "ipAddress": "95.31.18.119",
      "location": "Moskva, Russia, RU",
      "riskEventDateTime": "2016-02-03T05:20:33.7208156Z",
      "riskEventStatus": "active",
      "riskLevel": "low",
      "riskType": "MalwareRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89",
      "userPrincipalName": "jon@contoso.com"
    },
    {
      "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
      "closedDateTime": "2016-01-29T20:03:57.7872426Z",
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89-db69711e-9324-ec99-f010-6e63fb972e98",
      "ipAddress": "176.10.104.240",
      "location": "Bern, CH",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "remediated",
      "riskLevel": "medium",
      "riskType": "UnfamiliarLocationRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List identityRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
