---
title: Получение Компанинформатион
description: Возвращает объект сведений об Организации в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: ef94284b3c543868987a82a0f8422e9018060bdd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431965"
---
# <a name="get-companyinformation"></a><span data-ttu-id="23849-103">Получение Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="23849-103">Get companyInformation</span></span>

<span data-ttu-id="23849-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23849-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23849-105">Получение свойств и связей объекта сведений об организации для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="23849-105">Retrieve the properties and relationships of a company information object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="23849-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23849-106">Permissions</span></span>
<span data-ttu-id="23849-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23849-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23849-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23849-109">Permission type</span></span> |<span data-ttu-id="23849-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23849-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="23849-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23849-111">Delegated (work or school account)</span></span>|<span data-ttu-id="23849-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23849-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="23849-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23849-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="23849-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23849-114">Not supported.</span></span>|
|<span data-ttu-id="23849-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23849-115">Application</span></span>|<span data-ttu-id="23849-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23849-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23849-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23849-117">HTTP request</span></span>
```
GET /financials/companies/{id}/companyInformation/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="23849-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="23849-118">Optional query parameters</span></span>
<span data-ttu-id="23849-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="23849-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23849-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23849-120">Request headers</span></span>
|<span data-ttu-id="23849-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23849-121">Header</span></span>|<span data-ttu-id="23849-122">Значение</span><span class="sxs-lookup"><span data-stu-id="23849-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="23849-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23849-123">Authorization</span></span>  |<span data-ttu-id="23849-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23849-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23849-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="23849-126">Request body</span></span>
<span data-ttu-id="23849-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23849-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23849-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="23849-128">Response</span></span>
<span data-ttu-id="23849-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **компанинформатион** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23849-129">If successful, this method returns a `200 OK` response code and a **companyInformation** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23849-130">Пример</span><span class="sxs-lookup"><span data-stu-id="23849-130">Example</span></span>

<span data-ttu-id="23849-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="23849-131">**Request**</span></span>

<span data-ttu-id="23849-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23849-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/companyInformation/{id}
```

<span data-ttu-id="23849-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="23849-133">**Response**</span></span>

<span data-ttu-id="23849-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23849-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="23849-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="23849-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="23849-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="23849-136">All the properties will be returned from an actual call.</span></span>

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
