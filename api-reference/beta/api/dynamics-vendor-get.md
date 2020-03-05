---
title: Получение поставщиков
description: Возвращает объект Vendor в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 87c79a1b91044c23b771ca613e7b93ba79a1fed0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427916"
---
# <a name="get-vendors"></a><span data-ttu-id="fb320-103">Получение поставщиков</span><span class="sxs-lookup"><span data-stu-id="fb320-103">Get vendors</span></span>

<span data-ttu-id="fb320-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fb320-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb320-105">Получение свойств и связей объекта Vendor для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="fb320-105">Retrieve the properties and relationships of a vendor object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb320-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fb320-106">Permissions</span></span>
<span data-ttu-id="fb320-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb320-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb320-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb320-109">Permission type</span></span> |<span data-ttu-id="fb320-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb320-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="fb320-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb320-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb320-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb320-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="fb320-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb320-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="fb320-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb320-114">Not supported.</span></span>|
|<span data-ttu-id="fb320-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fb320-115">Application</span></span>|<span data-ttu-id="fb320-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb320-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb320-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb320-117">HTTP request</span></span>

```
GET /financials/companies/{id}/vendors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb320-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fb320-118">Optional query parameters</span></span>
<span data-ttu-id="fb320-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fb320-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb320-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fb320-120">Request headers</span></span>
|<span data-ttu-id="fb320-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb320-121">Header</span></span>|<span data-ttu-id="fb320-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fb320-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="fb320-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb320-123">Authorization</span></span>  |<span data-ttu-id="fb320-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb320-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb320-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb320-126">Request body</span></span>
<span data-ttu-id="fb320-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fb320-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb320-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb320-128">Response</span></span>
<span data-ttu-id="fb320-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **вендоров** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fb320-129">If successful, this method returns a `200 OK` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb320-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fb320-130">Example</span></span>

<span data-ttu-id="fb320-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="fb320-131">**Request**</span></span>

<span data-ttu-id="fb320-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb320-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/vendors/{id}
```

<span data-ttu-id="fb320-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="fb320-133">**Response**</span></span>

<span data-ttu-id="fb320-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fb320-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="fb320-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fb320-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fb320-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb320-136">All the properties will be returned from an actual call.</span></span>

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


