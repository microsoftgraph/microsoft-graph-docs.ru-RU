---
title: Создание клиентов
description: Создает объект клиента в Центре бизнеса Dynamics 365.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: e2426fdba7b41019e71cd7e4161d1d6fd2330433
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473394"
---
# <a name="create-customers"></a><span data-ttu-id="201f3-103">Создание клиентов</span><span class="sxs-lookup"><span data-stu-id="201f3-103">Create customers</span></span>

<span data-ttu-id="201f3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="201f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="201f3-105">Создание объекта клиента в Центре бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="201f3-105">Create a customer object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="201f3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="201f3-106">Permissions</span></span>
<span data-ttu-id="201f3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="201f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="201f3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="201f3-109">Permission type</span></span> |<span data-ttu-id="201f3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="201f3-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="201f3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="201f3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="201f3-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="201f3-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="201f3-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="201f3-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="201f3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="201f3-114">Not supported.</span></span>|
|<span data-ttu-id="201f3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="201f3-115">Application</span></span>|<span data-ttu-id="201f3-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="201f3-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="201f3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="201f3-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/customers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="201f3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="201f3-118">Optional query parameters</span></span>
<span data-ttu-id="201f3-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="201f3-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="201f3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="201f3-120">Request headers</span></span>
|<span data-ttu-id="201f3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="201f3-121">Header</span></span>         |<span data-ttu-id="201f3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="201f3-122">Value</span></span>                    |
|---------------|-------------------------|
|<span data-ttu-id="201f3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="201f3-123">Authorization</span></span>  |<span data-ttu-id="201f3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="201f3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="201f3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="201f3-126">Content-Type</span></span>   |<span data-ttu-id="201f3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="201f3-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="201f3-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="201f3-128">Request body</span></span>
<span data-ttu-id="201f3-129">В теле запроса поставляем JSON-представление объекта **клиентов.**</span><span class="sxs-lookup"><span data-stu-id="201f3-129">In the request body, supply a JSON representation of **customers** object.</span></span>

## <a name="response"></a><span data-ttu-id="201f3-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="201f3-130">Response</span></span>
<span data-ttu-id="201f3-131">В случае успешной работы этот метод возвращает код отклика и объект ```201 Created``` клиента в тексте ответа. </span><span class="sxs-lookup"><span data-stu-id="201f3-131">If successful, this method returns ```201 Created``` response code and a **customers** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="201f3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="201f3-132">Example</span></span>

<span data-ttu-id="201f3-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="201f3-133">**Request**</span></span>

<span data-ttu-id="201f3-134">Вот пример запроса.</span><span class="sxs-lookup"><span data-stu-id="201f3-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/customers
Content-type: application/json

{
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
  "overdueAmount": 0,
  "totalSalesExcludingTax": 0,
}

```

<span data-ttu-id="201f3-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="201f3-135">**Response**</span></span>

<span data-ttu-id="201f3-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="201f3-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="201f3-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="201f3-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="201f3-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="201f3-138">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

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
  "currencyCode": "USD",
  "blocked": " ",
  "balance": 0,
  "overdueAmount": 0,
  "totalSalesExcludingTax": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:28.983Z"
}

```



