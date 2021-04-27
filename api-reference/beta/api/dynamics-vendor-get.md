---
title: Получить поставщиков
description: Получает объект поставщика в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 6d701590a8a0d571075eca114930d0bfbdf5a50b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044825"
---
# <a name="get-vendors"></a><span data-ttu-id="e22fb-103">Получить поставщиков</span><span class="sxs-lookup"><span data-stu-id="e22fb-103">Get vendors</span></span>

<span data-ttu-id="e22fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e22fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e22fb-105">Извлечение свойств и связей объекта поставщика для Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="e22fb-105">Retrieve the properties and relationships of a vendor object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="e22fb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e22fb-106">Permissions</span></span>
<span data-ttu-id="e22fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e22fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e22fb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e22fb-109">Permission type</span></span> |<span data-ttu-id="e22fb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e22fb-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="e22fb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e22fb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e22fb-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e22fb-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="e22fb-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e22fb-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e22fb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e22fb-114">Not supported.</span></span>|
|<span data-ttu-id="e22fb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e22fb-115">Application</span></span>|<span data-ttu-id="e22fb-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e22fb-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e22fb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e22fb-117">HTTP request</span></span>

```http
GET /financials/companies/{id}/vendors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e22fb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e22fb-118">Optional query parameters</span></span>
<span data-ttu-id="e22fb-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e22fb-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e22fb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e22fb-120">Request headers</span></span>
|<span data-ttu-id="e22fb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e22fb-121">Header</span></span>|<span data-ttu-id="e22fb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e22fb-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="e22fb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e22fb-123">Authorization</span></span>  |<span data-ttu-id="e22fb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e22fb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e22fb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e22fb-126">Request body</span></span>
<span data-ttu-id="e22fb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e22fb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e22fb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e22fb-128">Response</span></span>
<span data-ttu-id="e22fb-129">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` поставщиков в  тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e22fb-129">If successful, this method returns a `200 OK` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e22fb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e22fb-130">Example</span></span>

<span data-ttu-id="e22fb-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="e22fb-131">**Request**</span></span>

<span data-ttu-id="e22fb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e22fb-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/vendors/{id}
```

<span data-ttu-id="e22fb-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="e22fb-133">**Response**</span></span>

<span data-ttu-id="e22fb-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e22fb-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="e22fb-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e22fb-135">**Note**: The response object shown here might be shortened for readability.</span></span>

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




