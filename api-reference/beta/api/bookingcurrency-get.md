---
title: Получение Букингкурренци
description: Получение свойств объекта Букингкурренци, доступного для корпоративных книг корпорации Майкрософт.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 7da9349dfbb1445072a0f399dbfd74431020b7d2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322317"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="d2f87-103">Получение Букингкурренци</span><span class="sxs-lookup"><span data-stu-id="d2f87-103">Get bookingCurrency</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2f87-104">Получение свойств объекта [букингкурренци](../resources/bookingcurrency.md) , доступного для корпоративных книг корпорации Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="d2f87-104">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="d2f87-105">Чтобы указать валюту, используйте свойство **ID** , которое является кодом валюты.</span><span class="sxs-lookup"><span data-stu-id="d2f87-105">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2f87-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2f87-106">Permissions</span></span>
<span data-ttu-id="d2f87-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2f87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2f87-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2f87-109">Permission type</span></span>      | <span data-ttu-id="d2f87-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2f87-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2f87-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2f87-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d2f87-112">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="d2f87-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d2f87-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2f87-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2f87-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f87-114">Not supported.</span></span>   |
|<span data-ttu-id="d2f87-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2f87-115">Application</span></span> | <span data-ttu-id="d2f87-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f87-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d2f87-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2f87-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d2f87-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d2f87-118">Optional query parameters</span></span>
<span data-ttu-id="d2f87-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d2f87-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2f87-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2f87-120">Request headers</span></span>
| <span data-ttu-id="d2f87-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d2f87-121">Name</span></span>      |<span data-ttu-id="d2f87-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d2f87-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d2f87-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2f87-123">Authorization</span></span>  | <span data-ttu-id="d2f87-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d2f87-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2f87-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2f87-125">Request body</span></span>
<span data-ttu-id="d2f87-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2f87-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d2f87-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2f87-127">Response</span></span>
<span data-ttu-id="d2f87-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [букингкурренци](../resources/bookingcurrency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d2f87-128">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2f87-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d2f87-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2f87-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2f87-130">Request</span></span>
<span data-ttu-id="d2f87-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2f87-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
##### <a name="response"></a><span data-ttu-id="d2f87-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2f87-132">Response</span></span>
<span data-ttu-id="d2f87-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2f87-133">The following is an example of the response.</span></span> <span data-ttu-id="d2f87-134">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="d2f87-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d2f87-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2f87-135">All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
