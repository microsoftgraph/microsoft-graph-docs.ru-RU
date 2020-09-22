---
title: Обновление Компанинформатион
description: Обновляет объект сведений о компании в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 72786990d20c4ca9be6d194494ac42b2b85a4c93
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008392"
---
# <a name="update-companyinformation"></a><span data-ttu-id="d8ed2-103">Обновление Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="d8ed2-103">Update companyInformation</span></span>

<span data-ttu-id="d8ed2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8ed2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8ed2-105">Обновление свойств объекта сведений об организации для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="d8ed2-105">Update the properties of a company information object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8ed2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8ed2-106">Permissions</span></span>
<span data-ttu-id="d8ed2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8ed2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8ed2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8ed2-109">Permission type</span></span> |<span data-ttu-id="d8ed2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8ed2-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d8ed2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8ed2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d8ed2-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8ed2-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d8ed2-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8ed2-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d8ed2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8ed2-114">Not supported.</span></span>|
|<span data-ttu-id="d8ed2-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d8ed2-115">Application</span></span>|<span data-ttu-id="d8ed2-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8ed2-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8ed2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8ed2-117">HTTP request</span></span>
```
PATCH /financials/companies/{id}/companyInformation/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d8ed2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d8ed2-118">Optional query parameters</span></span>
<span data-ttu-id="d8ed2-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d8ed2-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8ed2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8ed2-120">Request headers</span></span>
|<span data-ttu-id="d8ed2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8ed2-121">Header</span></span>        |<span data-ttu-id="d8ed2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d8ed2-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="d8ed2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8ed2-123">Authorization</span></span> |<span data-ttu-id="d8ed2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8ed2-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d8ed2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8ed2-126">Content-Type</span></span>  |<span data-ttu-id="d8ed2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d8ed2-127">application/json</span></span>         |
|<span data-ttu-id="d8ed2-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="d8ed2-128">If-Match</span></span>      |<span data-ttu-id="d8ed2-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8ed2-129">Required.</span></span> <span data-ttu-id="d8ed2-130">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **компанинформатион**, **компанинформатион** не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="d8ed2-130">When this request header is included and the eTag provided does not match the current tag on the **companyInformation**, the **companyInformation** will not be updated.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d8ed2-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8ed2-131">Request body</span></span>
<span data-ttu-id="d8ed2-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d8ed2-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="d8ed2-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8ed2-135">Response</span></span>
<span data-ttu-id="d8ed2-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект **компанинформатион** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d8ed2-136">If successful, this method returns a `200 OK` response code and an updated an **companyInformation** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8ed2-137">Пример</span><span class="sxs-lookup"><span data-stu-id="d8ed2-137">Example</span></span>

<span data-ttu-id="d8ed2-138">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="d8ed2-138">**Request**</span></span>

<span data-ttu-id="d8ed2-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8ed2-139">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/companyInformation/{id}
Content-type: application/json

{
  "displayName": "CRONUS USA, LTD.",
  "website": "www.cronuscorp.net"
}
```

<span data-ttu-id="d8ed2-140">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="d8ed2-140">**Response**</span></span>

<span data-ttu-id="d8ed2-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d8ed2-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="d8ed2-142">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d8ed2-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d8ed2-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8ed2-143">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "displayName": "CRONUS USA, LTD.",
  "address": {
    "street": "7122 South Ashford Street\r\nWestminster",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "+1 425 555 0100",
  "faxNumber": "+1 425 555 0101",
  "email": "",
  "website": "www.cronuscorp.net",
  "taxRegistrationNumber": "",
  "currencyCode": "USD",
  "currentFiscalYearStartDate": "2018-01-01",
  "industry": "",
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies/{id}/companyInformation/{id}/picture",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z"
  }
```


