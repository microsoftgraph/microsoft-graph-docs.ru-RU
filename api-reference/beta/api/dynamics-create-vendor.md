---
title: Создание поставщиков
description: Создает объект поставщика в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 24e0137e4d4979133ac03f98a0b58d599b018d9e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436437"
---
# <a name="create-vendors"></a><span data-ttu-id="5d3ea-103">Создание поставщиков</span><span class="sxs-lookup"><span data-stu-id="5d3ea-103">Create vendors</span></span>

<span data-ttu-id="5d3ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d3ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d3ea-105">Создание объекта поставщика в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="5d3ea-105">Create a vendor object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d3ea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5d3ea-106">Permissions</span></span>
<span data-ttu-id="5d3ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d3ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d3ea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d3ea-109">Permission type</span></span> |<span data-ttu-id="5d3ea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d3ea-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="5d3ea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d3ea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5d3ea-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d3ea-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="5d3ea-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d3ea-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5d3ea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d3ea-114">Not supported.</span></span>|
|<span data-ttu-id="5d3ea-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="5d3ea-115">Application</span></span>|<span data-ttu-id="5d3ea-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d3ea-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d3ea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d3ea-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/vendors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5d3ea-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5d3ea-118">Optional query parameters</span></span>
<span data-ttu-id="5d3ea-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5d3ea-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d3ea-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5d3ea-120">Request headers</span></span>
|<span data-ttu-id="5d3ea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5d3ea-121">Header</span></span>|<span data-ttu-id="5d3ea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5d3ea-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="5d3ea-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5d3ea-123">Authorization</span></span>  |<span data-ttu-id="5d3ea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d3ea-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="5d3ea-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d3ea-126">Content-Type</span></span>  |<span data-ttu-id="5d3ea-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5d3ea-127">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="5d3ea-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5d3ea-128">Request body</span></span>
<span data-ttu-id="5d3ea-129">В теле запроса поставляем представление JSON объекта **поставщиков.**</span><span class="sxs-lookup"><span data-stu-id="5d3ea-129">In the request body, supply a JSON representation of a **vendors** object.</span></span>

## <a name="response"></a><span data-ttu-id="5d3ea-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d3ea-130">Response</span></span>
<span data-ttu-id="5d3ea-131">В случае успешной работы этот метод возвращает код ответа и объект ```201 Created``` поставщиков в  тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5d3ea-131">If successful, this method returns ```201 Created``` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d3ea-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5d3ea-132">Example</span></span>

<span data-ttu-id="5d3ea-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="5d3ea-133">**Request**</span></span>

<span data-ttu-id="5d3ea-134">Вот пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d3ea-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/vendors
Content-type: application/json

{
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
  "currencyCode": "USD",
  "irs1099Code": "",
  "taxLiable": true,
  "blocked": " "
}
```

<span data-ttu-id="5d3ea-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="5d3ea-135">**Response**</span></span>

<span data-ttu-id="5d3ea-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5d3ea-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="5d3ea-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5d3ea-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5d3ea-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d3ea-138">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "40000",
  "displayName": "Wide World Importers",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z"
}
```



