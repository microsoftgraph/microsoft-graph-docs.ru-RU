---
title: Получение клиентов
description: Возвращает объект Customer в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0512a493032e738bba41362ecdc40e78de951baf
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365845"
---
# <a name="get-customers"></a><span data-ttu-id="b0339-103">Получение клиентов</span><span class="sxs-lookup"><span data-stu-id="b0339-103">Get customers</span></span>
<span data-ttu-id="b0339-104">Получение свойств и связей объекта Customer для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="b0339-104">Retrieve the properties and relationships of a customer object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0339-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0339-105">Permissions</span></span>
<span data-ttu-id="b0339-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0339-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0339-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0339-108">Permission type</span></span> |<span data-ttu-id="b0339-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0339-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="b0339-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0339-110">Delegated (work or school account)</span></span>|<span data-ttu-id="b0339-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0339-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="b0339-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0339-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b0339-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0339-113">Not supported.</span></span>|
|<span data-ttu-id="b0339-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0339-114">Application</span></span>|<span data-ttu-id="b0339-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0339-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0339-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0339-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/customers('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0339-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b0339-117">Optional query parameters</span></span>
<span data-ttu-id="b0339-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b0339-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0339-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0339-119">Request headers</span></span>
|<span data-ttu-id="b0339-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b0339-120">Header</span></span>|<span data-ttu-id="b0339-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b0339-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="b0339-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0339-122">Authorization</span></span>  |<span data-ttu-id="b0339-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b0339-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0339-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0339-125">Request body</span></span>
<span data-ttu-id="b0339-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b0339-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0339-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0339-127">Response</span></span>
<span data-ttu-id="b0339-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **Customers** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b0339-128">If successful, this method returns a `200 OK` response code and a **customers** object in the response body.</span></span>

<span data-ttu-id="b0339-129">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="b0339-129">**Request**</span></span>

<span data-ttu-id="b0339-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0339-130">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/customers('{id}')
```

<span data-ttu-id="b0339-131">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="b0339-131">**Response**</span></span>

<span data-ttu-id="b0339-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b0339-132">Here is an example of the response.</span></span> 

> <span data-ttu-id="b0339-133">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b0339-133">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b0339-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b0339-134">All the properties will be returned from an actual call.</span></span>

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

