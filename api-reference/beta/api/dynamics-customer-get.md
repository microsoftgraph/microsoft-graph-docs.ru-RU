---
title: Получение клиентов
description: Возвращает объект Customer в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 32ec34526a6bbb31191b6a8b86f9ea039e507d04
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42430849"
---
# <a name="get-customers"></a><span data-ttu-id="10101-103">Получение клиентов</span><span class="sxs-lookup"><span data-stu-id="10101-103">Get customers</span></span>

<span data-ttu-id="10101-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="10101-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10101-105">Получение свойств и связей объекта Customer для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="10101-105">Retrieve the properties and relationships of a customer object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="10101-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10101-106">Permissions</span></span>
<span data-ttu-id="10101-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10101-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10101-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10101-109">Permission type</span></span> |<span data-ttu-id="10101-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10101-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="10101-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10101-111">Delegated (work or school account)</span></span>|<span data-ttu-id="10101-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10101-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="10101-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10101-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="10101-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10101-114">Not supported.</span></span>|
|<span data-ttu-id="10101-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10101-115">Application</span></span>|<span data-ttu-id="10101-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10101-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10101-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10101-117">HTTP request</span></span>
```
GET /financials/companies/{id}/customers/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10101-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="10101-118">Optional query parameters</span></span>
<span data-ttu-id="10101-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="10101-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10101-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10101-120">Request headers</span></span>
|<span data-ttu-id="10101-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="10101-121">Header</span></span>|<span data-ttu-id="10101-122">Значение</span><span class="sxs-lookup"><span data-stu-id="10101-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="10101-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="10101-123">Authorization</span></span>  |<span data-ttu-id="10101-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10101-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10101-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10101-126">Request body</span></span>
<span data-ttu-id="10101-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10101-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10101-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="10101-128">Response</span></span>
<span data-ttu-id="10101-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **Customers** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10101-129">If successful, this method returns a `200 OK` response code and a **customers** object in the response body.</span></span>

<span data-ttu-id="10101-130">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="10101-130">**Request**</span></span>

<span data-ttu-id="10101-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10101-131">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/customers/{id}
```

<span data-ttu-id="10101-132">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="10101-132">**Response**</span></span>

<span data-ttu-id="10101-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10101-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="10101-134">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="10101-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="10101-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10101-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "number": "10000",
  "displayName": "Coho Winery",
  "type": "Company",
  "address": {
    "street": "192 Market Square",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "",
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
  "paymentMethodId": "paymentMethodId-value",
  "blocked": " ",
  "balance": 0,
  "overdueAmount": 0,
  "totalSalesExcludingTax": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:28.983Z"
}
```

