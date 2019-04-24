---
title: Получение Компанинформатион
description: Возвращает объект сведений об Организации в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ad49c3d4095283fc42c2e8f2046c646f3558ac18
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454190"
---
# <a name="get-companyinformation"></a><span data-ttu-id="2f078-103">Получение Компанинформатион</span><span class="sxs-lookup"><span data-stu-id="2f078-103">Get companyInformation</span></span>
<span data-ttu-id="2f078-104">Получение свойств и связей объекта сведений об организации для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="2f078-104">Retrieve the properties and relationships of a company information object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f078-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f078-105">Permissions</span></span>
<span data-ttu-id="2f078-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f078-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f078-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f078-108">Permission type</span></span> |<span data-ttu-id="2f078-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f078-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="2f078-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f078-110">Delegated (work or school account)</span></span>|<span data-ttu-id="2f078-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f078-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="2f078-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f078-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2f078-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f078-113">Not supported.</span></span>|
|<span data-ttu-id="2f078-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f078-114">Application</span></span>|<span data-ttu-id="2f078-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f078-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f078-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f078-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/companyInformation('{id}')
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2f078-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2f078-117">Optional query parameters</span></span>
<span data-ttu-id="2f078-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2f078-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f078-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f078-119">Request headers</span></span>
|<span data-ttu-id="2f078-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f078-120">Header</span></span>|<span data-ttu-id="2f078-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2f078-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="2f078-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f078-122">Authorization</span></span>  |<span data-ttu-id="2f078-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f078-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f078-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f078-125">Request body</span></span>
<span data-ttu-id="2f078-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f078-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f078-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f078-127">Response</span></span>
<span data-ttu-id="2f078-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **компанинформатион** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f078-128">If successful, this method returns a `200 OK` response code and a **companyInformation** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f078-129">Пример</span><span class="sxs-lookup"><span data-stu-id="2f078-129">Example</span></span>

<span data-ttu-id="2f078-130">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="2f078-130">**Request**</span></span>

<span data-ttu-id="2f078-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f078-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/companyInformation('{id}')
```

<span data-ttu-id="2f078-132">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="2f078-132">**Response**</span></span>

<span data-ttu-id="2f078-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2f078-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="2f078-134">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2f078-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2f078-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f078-135">All the properties will be returned from an actual call.</span></span>

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
  "picture@odata.mediaReadLink": "https://api.financials.dynamics.com/v1.0/api/beta/companies('{id}')/companyInformation('{id}')/picture",
  "businessProfileId": "",
  "lastModifiedDateTime": "2017-03-16T14:57:19.497Z"
}
```
