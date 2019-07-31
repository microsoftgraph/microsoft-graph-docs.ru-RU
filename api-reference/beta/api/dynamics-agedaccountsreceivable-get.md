---
title: Получение Ажедаккаунтсрецеивабле
description: Получает объект устаревших расчетов с клиентами в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.author: solsen
doc_type: apiPageType
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 3e23ea971ad16d32d3a651259818524870abedc2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956851"
---
# <a name="get-agedaccountsreceivable"></a><span data-ttu-id="17a44-103">Получение Ажедаккаунтсрецеивабле</span><span class="sxs-lookup"><span data-stu-id="17a44-103">Get agedAccountsReceivable</span></span>
<span data-ttu-id="17a44-104">Получение свойств и связей для устаревших объектов отчета о расчетах с поставщиками для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="17a44-104">Retrieve the properties and relationships of an aged accounts receivable report object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="17a44-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="17a44-105">Permissions</span></span>
<span data-ttu-id="17a44-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17a44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17a44-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17a44-108">Permission type</span></span> |<span data-ttu-id="17a44-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17a44-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="17a44-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17a44-110">Delegated (work or school account)</span></span>|<span data-ttu-id="17a44-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17a44-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="17a44-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17a44-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="17a44-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17a44-113">Not supported.</span></span>|
|<span data-ttu-id="17a44-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17a44-114">Application</span></span>|<span data-ttu-id="17a44-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17a44-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="17a44-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17a44-116">HTTP request</span></span>
```
GET /financials/companies('{id}')/agedAccountsReceivable
```
## <a name="optional-query-parameters"></a><span data-ttu-id="17a44-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="17a44-117">Optional query parameters</span></span>
<span data-ttu-id="17a44-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="17a44-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17a44-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17a44-119">Request headers</span></span>
|<span data-ttu-id="17a44-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17a44-120">Header</span></span>|<span data-ttu-id="17a44-121">Значение</span><span class="sxs-lookup"><span data-stu-id="17a44-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="17a44-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17a44-122">Authorization</span></span>  |<span data-ttu-id="17a44-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17a44-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17a44-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="17a44-125">Request body</span></span>
<span data-ttu-id="17a44-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="17a44-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17a44-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="17a44-127">Response</span></span>
<span data-ttu-id="17a44-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **ажедаккаунтсрецеивабле** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="17a44-128">If successful, this method returns a `200 OK` response code and an **agedAccountsReceivable** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17a44-129">Пример</span><span class="sxs-lookup"><span data-stu-id="17a44-129">Example</span></span>

<span data-ttu-id="17a44-130">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="17a44-130">**Request**</span></span>

<span data-ttu-id="17a44-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17a44-131">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/agedAccountsReceivable?$filter=periodLengthFilter eq '3M'
```

<span data-ttu-id="17a44-132">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="17a44-132">**Response**</span></span>

<span data-ttu-id="17a44-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="17a44-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="17a44-134">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="17a44-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="17a44-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17a44-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "customerId": "id-value",
  "customerNumber": "30000",
  "name": "Relecloud",
  "currencyCode": "USD",
  "balanceDue": 349615.45,
  "currentAmount": 0,
  "period1Amount": 349615.45,
  "period2Amount": 0,
  "period3Amount": 0,
  "agedAsOfDate": "2017-04-25",
  "periodLengthFilter": "3M"   
}
```
