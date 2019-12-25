---
title: Получение объекта identityRiskEvent
description: Получение свойств и связей объекта идентитирискевент.
author: cloudhandler
localization_priority: Normal
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: dd97464336dda8846cb34baef0a03f1490cfae3a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869558"
---
# <a name="get-identityriskevent"></a><span data-ttu-id="47a0c-103">Получение объекта identityRiskEvent</span><span class="sxs-lookup"><span data-stu-id="47a0c-103">Get identityRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="47a0c-104">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="47a0c-104">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="47a0c-105">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="47a0c-105">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="47a0c-106">Получение свойств и связей объекта идентитирискевент.</span><span class="sxs-lookup"><span data-stu-id="47a0c-106">Retrieve the properties and relationships of identityriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="47a0c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47a0c-107">Permissions</span></span>
<span data-ttu-id="47a0c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47a0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47a0c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47a0c-110">Permission type</span></span>      | <span data-ttu-id="47a0c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47a0c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47a0c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47a0c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="47a0c-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="47a0c-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="47a0c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47a0c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47a0c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47a0c-115">Not supported.</span></span>    |
|<span data-ttu-id="47a0c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="47a0c-116">Application</span></span> | <span data-ttu-id="47a0c-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="47a0c-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47a0c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47a0c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="47a0c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47a0c-119">Request headers</span></span>
| <span data-ttu-id="47a0c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="47a0c-120">Name</span></span>      |<span data-ttu-id="47a0c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="47a0c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="47a0c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47a0c-122">Authorization</span></span>  | <span data-ttu-id="47a0c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47a0c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47a0c-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="47a0c-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="47a0c-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="47a0c-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47a0c-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="47a0c-128">Request body</span></span>
<span data-ttu-id="47a0c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47a0c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47a0c-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="47a0c-130">Response</span></span>

<span data-ttu-id="47a0c-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [идентитирискевент](../resources/identityriskevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47a0c-131">If successful, this method returns a `200 OK` response code and [identityRiskEvent](../resources/identityriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="47a0c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="47a0c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47a0c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="47a0c-133">Request</span></span>
<span data-ttu-id="47a0c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47a0c-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="47a0c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="47a0c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityriskevent"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityRiskEvents/ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-c2b6c2b9-dddc-acd0-2b39-d519d803dbc3-db69711e-9324-ec99-f010-6e63fb972e98
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="47a0c-136">C#</span><span class="sxs-lookup"><span data-stu-id="47a0c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityriskevent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="47a0c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47a0c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityriskevent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="47a0c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47a0c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityriskevent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="47a0c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="47a0c-139">Response</span></span>
<span data-ttu-id="47a0c-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47a0c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get identityRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
