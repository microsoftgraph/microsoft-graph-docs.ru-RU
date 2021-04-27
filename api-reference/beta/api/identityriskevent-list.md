---
title: List identityRiskEvents
description: Извлечение списка объектов identityriskevent.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 00aa8a68af191478fc9de73b865050ba441e0e3d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040821"
---
# <a name="list-identityriskevents-deprecated"></a><span data-ttu-id="1fd30-103">List identityRiskEvents (deprecated)</span><span class="sxs-lookup"><span data-stu-id="1fd30-103">List identityRiskEvents (deprecated)</span></span>

<span data-ttu-id="1fd30-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fd30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
><span data-ttu-id="1fd30-105">API **identityRiskEvents** обесценен и прекратит возвращать данные 10 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="1fd30-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="1fd30-106">Подробные сведения см. в материале [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="1fd30-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="1fd30-107">Извлечение списка объектов identityriskevent.</span><span class="sxs-lookup"><span data-stu-id="1fd30-107">Retrieve a list of identityriskevent objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fd30-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1fd30-108">Permissions</span></span>
<span data-ttu-id="1fd30-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fd30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fd30-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fd30-111">Permission type</span></span>      | <span data-ttu-id="1fd30-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fd30-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fd30-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fd30-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1fd30-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fd30-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="1fd30-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fd30-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fd30-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fd30-116">Not supported.</span></span>    |
|<span data-ttu-id="1fd30-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1fd30-117">Application</span></span> | <span data-ttu-id="1fd30-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fd30-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fd30-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fd30-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="1fd30-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1fd30-120">Request headers</span></span>
| <span data-ttu-id="1fd30-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1fd30-121">Name</span></span>      |<span data-ttu-id="1fd30-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1fd30-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1fd30-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1fd30-123">Authorization</span></span>  | <span data-ttu-id="1fd30-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fd30-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1fd30-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="1fd30-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="1fd30-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="1fd30-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fd30-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1fd30-129">Request body</span></span>
<span data-ttu-id="1fd30-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1fd30-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fd30-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fd30-131">Response</span></span>

<span data-ttu-id="1fd30-132">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [identityRiskEvent](../resources/identityriskevent.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1fd30-132">If successful, this method returns a `200 OK` response code and collection of [identityRiskEvent](../resources/identityriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1fd30-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1fd30-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1fd30-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fd30-134">Request</span></span>
<span data-ttu-id="1fd30-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fd30-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1fd30-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fd30-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityriskevents"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityRiskEvents
```
# <a name="c"></a>[<span data-ttu-id="1fd30-137">C#</span><span class="sxs-lookup"><span data-stu-id="1fd30-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityriskevents-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fd30-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fd30-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityriskevents-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fd30-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fd30-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityriskevents-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1fd30-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fd30-140">Response</span></span>
<span data-ttu-id="1fd30-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1fd30-141">Here is an example of the response.</span></span> <span data-ttu-id="1fd30-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1fd30-142">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List identityRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


