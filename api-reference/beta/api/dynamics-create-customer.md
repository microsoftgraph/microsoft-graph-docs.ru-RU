---
title: Создание клиентов
description: Создает объект Customer в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 549c17420790bb0146c4a84b0a5b3a49ca9e3ec9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431734"
---
# <a name="create-customers"></a><span data-ttu-id="5e696-103">Создание клиентов</span><span class="sxs-lookup"><span data-stu-id="5e696-103">Create customers</span></span>

<span data-ttu-id="5e696-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e696-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e696-105">Создайте объект Customer в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="5e696-105">Create a customer object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e696-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e696-106">Permissions</span></span>
<span data-ttu-id="5e696-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e696-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e696-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e696-109">Permission type</span></span> |<span data-ttu-id="5e696-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e696-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="5e696-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e696-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5e696-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e696-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="5e696-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e696-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5e696-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e696-114">Not supported.</span></span>|
|<span data-ttu-id="5e696-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e696-115">Application</span></span>|<span data-ttu-id="5e696-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e696-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e696-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e696-117">HTTP request</span></span>
```
POST /financials/companies/{id}/customers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5e696-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5e696-118">Optional query parameters</span></span>
<span data-ttu-id="5e696-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5e696-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e696-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e696-120">Request headers</span></span>
|<span data-ttu-id="5e696-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e696-121">Header</span></span>         |<span data-ttu-id="5e696-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5e696-122">Value</span></span>                    |
|---------------|-------------------------|
|<span data-ttu-id="5e696-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e696-123">Authorization</span></span>  |<span data-ttu-id="5e696-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e696-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5e696-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e696-126">Content-Type</span></span>   |<span data-ttu-id="5e696-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5e696-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="5e696-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5e696-128">Request body</span></span>
<span data-ttu-id="5e696-129">В тексте запроса добавьте представление объекта **Customers** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e696-129">In the request body, supply a JSON representation of **customers** object.</span></span>

## <a name="response"></a><span data-ttu-id="5e696-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e696-130">Response</span></span>
<span data-ttu-id="5e696-131">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **Customers** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e696-131">If successful, this method returns ```201 Created``` response code and a **customers** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e696-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5e696-132">Example</span></span>

<span data-ttu-id="5e696-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="5e696-133">**Request**</span></span>

<span data-ttu-id="5e696-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e696-134">Here is an example of a request.</span></span>

```json
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

<span data-ttu-id="5e696-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="5e696-135">**Response**</span></span>

<span data-ttu-id="5e696-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5e696-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="5e696-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5e696-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5e696-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e696-138">All the properties will be returned from an actual call.</span></span>

```json
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

