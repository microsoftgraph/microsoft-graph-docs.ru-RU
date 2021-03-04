---
title: Получить поставщиков
description: Получает объект поставщика в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 036454a27b2d363a328fca73ce54c9ce112b566d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436430"
---
# <a name="get-vendors"></a><span data-ttu-id="e5754-103">Получить поставщиков</span><span class="sxs-lookup"><span data-stu-id="e5754-103">Get vendors</span></span>

<span data-ttu-id="e5754-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5754-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5754-105">Извлечение свойств и связей объекта поставщика для Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="e5754-105">Retrieve the properties and relationships of a vendor object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5754-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5754-106">Permissions</span></span>
<span data-ttu-id="e5754-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5754-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5754-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5754-109">Permission type</span></span> |<span data-ttu-id="e5754-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5754-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="e5754-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5754-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e5754-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5754-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="e5754-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5754-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e5754-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5754-114">Not supported.</span></span>|
|<span data-ttu-id="e5754-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="e5754-115">Application</span></span>|<span data-ttu-id="e5754-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5754-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5754-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5754-117">HTTP request</span></span>

```http
GET /financials/companies/{id}/vendors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5754-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e5754-118">Optional query parameters</span></span>
<span data-ttu-id="e5754-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e5754-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e5754-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5754-120">Request headers</span></span>
|<span data-ttu-id="e5754-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5754-121">Header</span></span>|<span data-ttu-id="e5754-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e5754-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="e5754-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5754-123">Authorization</span></span>  |<span data-ttu-id="e5754-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5754-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5754-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e5754-126">Request body</span></span>
<span data-ttu-id="e5754-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5754-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5754-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5754-128">Response</span></span>
<span data-ttu-id="e5754-129">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` поставщиков в  тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e5754-129">If successful, this method returns a `200 OK` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5754-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e5754-130">Example</span></span>

<span data-ttu-id="e5754-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="e5754-131">**Request**</span></span>

<span data-ttu-id="e5754-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5754-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/vendors/{id}
```

<span data-ttu-id="e5754-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="e5754-133">**Response**</span></span>

<span data-ttu-id="e5754-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e5754-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="e5754-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e5754-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e5754-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e5754-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "number": "40000",
  "displayName": "Wide World Importers",
  "address": {
    "street": "51 Radcroft Road",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "",
  "email": "toby.rhode@cronuscorp.net",
  "website": "",
  "taxRegistrationNumber": "",
  "currencyId": "id-value",
  "currencyCode": "USD",
  "irs1099Code": "",
  "paymentTermsId": "id-value",
  "paymentMethodId": "id-value",
  "taxLiable": true,
  "blocked": " ",
  "balance": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:29.667Z"
}
```




