---
title: Получение Компанинформатион
description: Возвращает объект сведений об Организации в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 0f98b395182a5b0acaf122bf0973c5904cc9e5d4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981746"
---
# <a name="get-companyinformation"></a><span data-ttu-id="1e4f8-103">Получение Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="1e4f8-103">Get companyInformation</span></span>

<span data-ttu-id="1e4f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e4f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e4f8-105">Получение свойств и связей объекта сведений об организации для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="1e4f8-105">Retrieve the properties and relationships of a company information object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e4f8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1e4f8-106">Permissions</span></span>
<span data-ttu-id="1e4f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e4f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e4f8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1e4f8-109">Permission type</span></span> |<span data-ttu-id="1e4f8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1e4f8-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="1e4f8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1e4f8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1e4f8-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e4f8-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="1e4f8-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1e4f8-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="1e4f8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e4f8-114">Not supported.</span></span>|
|<span data-ttu-id="1e4f8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1e4f8-115">Application</span></span>|<span data-ttu-id="1e4f8-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e4f8-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e4f8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1e4f8-117">HTTP request</span></span>
```
GET /financials/companies/{id}/companyInformation/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1e4f8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1e4f8-118">Optional query parameters</span></span>
<span data-ttu-id="1e4f8-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1e4f8-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e4f8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1e4f8-120">Request headers</span></span>
|<span data-ttu-id="1e4f8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1e4f8-121">Header</span></span>|<span data-ttu-id="1e4f8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1e4f8-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="1e4f8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1e4f8-123">Authorization</span></span>  |<span data-ttu-id="1e4f8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1e4f8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e4f8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1e4f8-126">Request body</span></span>
<span data-ttu-id="1e4f8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1e4f8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e4f8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e4f8-128">Response</span></span>
<span data-ttu-id="1e4f8-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **компанинформатион** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1e4f8-129">If successful, this method returns a `200 OK` response code and a **companyInformation** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e4f8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1e4f8-130">Example</span></span>

<span data-ttu-id="1e4f8-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="1e4f8-131">**Request**</span></span>

<span data-ttu-id="1e4f8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1e4f8-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/companyInformation/{id}
```

<span data-ttu-id="1e4f8-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="1e4f8-133">**Response**</span></span>

<span data-ttu-id="1e4f8-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1e4f8-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="1e4f8-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1e4f8-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1e4f8-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1e4f8-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "displayName": "CRONUS USA, Inc.",
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
  "website": "",
  "taxRegistrationNumber": "",
  "currencyCode": "USD",
  "currentFiscalYearStartDate": "2018-01-01",
  "industry": "",
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies/{id}/companyInformation/{id}/picture",
  "businessProfileId": "",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z"
}
```


