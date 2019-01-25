---
title: Получение bookingCurrency
description: Получение свойств объекта bookingCurrency, доступные для резервирования Microsoft business.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b4fd1cf854d84001d58a64dac18ca7fb276e6efa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524228"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="dedd2-103">Получение bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="dedd2-103">Get bookingCurrency</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dedd2-104">Получение свойств объекта [bookingCurrency](../resources/bookingcurrency.md) , доступные для резервирования Microsoft business.</span><span class="sxs-lookup"><span data-stu-id="dedd2-104">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="dedd2-105">Используйте свойство **id** , которая код валюты, чтобы указать валюты.</span><span class="sxs-lookup"><span data-stu-id="dedd2-105">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="dedd2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dedd2-106">Permissions</span></span>
<span data-ttu-id="dedd2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dedd2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dedd2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dedd2-109">Permission type</span></span>      | <span data-ttu-id="dedd2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dedd2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dedd2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dedd2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dedd2-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="dedd2-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="dedd2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dedd2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dedd2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dedd2-114">Not supported.</span></span>   |
|<span data-ttu-id="dedd2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dedd2-115">Application</span></span> | <span data-ttu-id="dedd2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dedd2-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="dedd2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dedd2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dedd2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dedd2-118">Optional query parameters</span></span>
<span data-ttu-id="dedd2-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dedd2-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dedd2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dedd2-120">Request headers</span></span>
| <span data-ttu-id="dedd2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="dedd2-121">Name</span></span>      |<span data-ttu-id="dedd2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dedd2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dedd2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dedd2-123">Authorization</span></span>  | <span data-ttu-id="dedd2-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="dedd2-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="dedd2-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dedd2-125">Request body</span></span>
<span data-ttu-id="dedd2-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dedd2-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="dedd2-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="dedd2-127">Response</span></span>
<span data-ttu-id="dedd2-128">Успешно завершена, этот метод возвращает `200 OK` объект [bookingCurrency](../resources/bookingcurrency.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dedd2-128">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dedd2-129">Пример</span><span class="sxs-lookup"><span data-stu-id="dedd2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dedd2-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="dedd2-130">Request</span></span>
<span data-ttu-id="dedd2-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dedd2-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
##### <a name="response"></a><span data-ttu-id="dedd2-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="dedd2-132">Response</span></span>
<span data-ttu-id="dedd2-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dedd2-133">The following is an example of the response.</span></span> <span data-ttu-id="dedd2-134">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="dedd2-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dedd2-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dedd2-135">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingcurrency-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
