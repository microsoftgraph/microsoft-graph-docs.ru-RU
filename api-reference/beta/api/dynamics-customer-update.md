---
title: Обновление клиентов
description: Обновляет объект клиента в Центре бизнеса Dynamics 365.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: e19c24cd453a5702e64019e6fb96903786d41a19
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045630"
---
# <a name="update-customers"></a><span data-ttu-id="08675-103">Обновление клиентов</span><span class="sxs-lookup"><span data-stu-id="08675-103">Update customers</span></span>

<span data-ttu-id="08675-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08675-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08675-105">Обновление свойств объекта клиента для Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="08675-105">Update the properties of a customer object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="08675-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08675-106">Permissions</span></span>
<span data-ttu-id="08675-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08675-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08675-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08675-109">Permission type</span></span> |<span data-ttu-id="08675-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08675-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="08675-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08675-111">Delegated (work or school account)</span></span>|<span data-ttu-id="08675-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08675-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="08675-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08675-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="08675-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08675-114">Not supported.</span></span>|
|<span data-ttu-id="08675-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08675-115">Application</span></span>|<span data-ttu-id="08675-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08675-116">Financials.ReadWrite.All</span></span>|
## <a name="http-request"></a><span data-ttu-id="08675-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08675-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/customers/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="08675-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="08675-118">Optional query parameters</span></span>
<span data-ttu-id="08675-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="08675-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08675-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08675-120">Request headers</span></span>
|<span data-ttu-id="08675-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08675-121">Header</span></span>         |<span data-ttu-id="08675-122">Значение</span><span class="sxs-lookup"><span data-stu-id="08675-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="08675-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08675-123">Authorization</span></span>  |<span data-ttu-id="08675-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08675-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="08675-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08675-126">Content-Type</span></span>   |<span data-ttu-id="08675-127">application/json.</span><span class="sxs-lookup"><span data-stu-id="08675-127">application/json.</span></span>         |
|<span data-ttu-id="08675-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="08675-128">If-Match</span></span>       |<span data-ttu-id="08675-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08675-129">Required.</span></span> <span data-ttu-id="08675-130">Если этот заглавный запрос включен и предоставленный eTag не совпадает с текущим тегом для **клиентов,** клиенты не будут обновляться. </span><span class="sxs-lookup"><span data-stu-id="08675-130">When this request header is included and the eTag provided does not match the current tag on the **customers**, the **customers** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08675-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08675-131">Request body</span></span>
<span data-ttu-id="08675-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="08675-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="08675-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="08675-135">Response</span></span>
<span data-ttu-id="08675-136">В случае успешной работы этот метод возвращает код отклика и обновленный объект клиентов `200 OK` в тексте  ответа.</span><span class="sxs-lookup"><span data-stu-id="08675-136">If successful, this method returns a `200 OK` response code and an updated **customers** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08675-137">Пример</span><span class="sxs-lookup"><span data-stu-id="08675-137">Example</span></span>

<span data-ttu-id="08675-138">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="08675-138">**Request**</span></span>

<span data-ttu-id="08675-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08675-139">Here is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/customers/{id}
Content-type: application/json

{
  "displayName": "Coho Winery Inc.",
  "phoneNumber": "(555) 555-1234"
}
```

<span data-ttu-id="08675-140">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="08675-140">**Response**</span></span>

<span data-ttu-id="08675-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="08675-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="08675-142">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="08675-142">**Note**: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "number": "10000",
  "displayName": "Coho Winery Inc.",
  "type": "Company",
  "address": {
    "street": "192 Market Square",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "(555) 555-1234"
  "email": "jim.glynn@cronuscorp.net",
  "website": "",
  "taxLiable": true,
  "taxAreaId": "taxAreaId-value",
  "taxAreaDisplayName": "tax area",
  "taxRegistrationNumber": "28012001T",
  "currencyId": "currencyId-value",
  "currencyCode": "USD",
  "paymentTermsId": "paymentTermsId-value",
  "shipmentMethodId": "shipmentMethodId-value",
  "paymentMethodId": "paymentMethod-value",
  "blocked": " ",
  "balance": 0,
  "overdueAmount": 0
  "totalSalesExcludingTax": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:28.983Z"
}
```




