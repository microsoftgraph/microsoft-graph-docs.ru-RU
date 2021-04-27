---
title: Получить bookingCurrency
description: Получите свойства объекта bookingCurrency, доступного для бизнеса Microsoft Bookings.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: f6702d108c3b705749021ad79d7e9fe6ceb944b1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047842"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="8e453-103">Получить bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="8e453-103">Get bookingCurrency</span></span>

<span data-ttu-id="8e453-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e453-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e453-105">Получите свойства объекта [bookingCurrency,](../resources/bookingcurrency.md) доступного для бизнеса Microsoft Bookings.</span><span class="sxs-lookup"><span data-stu-id="8e453-105">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="8e453-106">Чтобы указать валюту, используйте свойство **id,** которое является кодом валюты.</span><span class="sxs-lookup"><span data-stu-id="8e453-106">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e453-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e453-107">Permissions</span></span>
<span data-ttu-id="8e453-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e453-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e453-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e453-110">Permission type</span></span>      | <span data-ttu-id="8e453-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e453-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e453-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e453-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8e453-113">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="8e453-113">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="8e453-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e453-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e453-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e453-115">Not supported.</span></span>   |
|<span data-ttu-id="8e453-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e453-116">Application</span></span> | <span data-ttu-id="8e453-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e453-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="8e453-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e453-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8e453-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8e453-119">Optional query parameters</span></span>
<span data-ttu-id="8e453-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8e453-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e453-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e453-121">Request headers</span></span>
| <span data-ttu-id="8e453-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8e453-122">Name</span></span>      |<span data-ttu-id="8e453-123">Описание</span><span class="sxs-lookup"><span data-stu-id="8e453-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8e453-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e453-124">Authorization</span></span>  | <span data-ttu-id="8e453-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8e453-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e453-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e453-126">Request body</span></span>
<span data-ttu-id="8e453-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8e453-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8e453-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e453-128">Response</span></span>
<span data-ttu-id="8e453-129">В случае успеха этот метод возвращает код отклика и `200 OK` [объект bookingCurrency](../resources/bookingcurrency.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8e453-129">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8e453-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8e453-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e453-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e453-131">Request</span></span>
<span data-ttu-id="8e453-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e453-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e453-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e453-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
# <a name="c"></a>[<span data-ttu-id="8e453-134">C#</span><span class="sxs-lookup"><span data-stu-id="8e453-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcurrency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e453-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e453-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcurrency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e453-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e453-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcurrency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e453-137">Java</span><span class="sxs-lookup"><span data-stu-id="8e453-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingcurrency-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8e453-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e453-138">Response</span></span>
<span data-ttu-id="8e453-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8e453-139">The following is an example of the response.</span></span> <span data-ttu-id="8e453-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8e453-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCurrency"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 50

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingCurrencies/$entity",
    "id": "USD",
    "symbol": "$"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingCurrency",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
