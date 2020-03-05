---
title: Получение Ажедаккаунтспайабле
description: Возвращает устаревший объект кредиторской задолженности в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 36f8c82fc832eafa538c8a913cfb5863d2a1606f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42432098"
---
# <a name="get-agedaccountspayable"></a><span data-ttu-id="3581f-103">Получение Ажедаккаунтспайабле</span><span class="sxs-lookup"><span data-stu-id="3581f-103">Get agedAccountsPayable</span></span>

<span data-ttu-id="3581f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3581f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3581f-105">Получение свойств и связей для устаревших отчетов об оплате учетных записей для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="3581f-105">Retrieve the properties and relationships of an aged accounts payable report object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="3581f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3581f-106">Permissions</span></span>
<span data-ttu-id="3581f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3581f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3581f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3581f-109">Permission type</span></span> |<span data-ttu-id="3581f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3581f-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="3581f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3581f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3581f-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3581f-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="3581f-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3581f-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3581f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3581f-114">Not supported.</span></span>|
|<span data-ttu-id="3581f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3581f-115">Application</span></span>|<span data-ttu-id="3581f-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3581f-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3581f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3581f-117">HTTP request</span></span>
```
GET /financials/companies/{id}/agedAccountsPayable
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3581f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3581f-118">Optional query parameters</span></span>
<span data-ttu-id="3581f-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3581f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3581f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3581f-120">Request headers</span></span>
|<span data-ttu-id="3581f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3581f-121">Header</span></span>        |<span data-ttu-id="3581f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3581f-122">Value</span></span>                     |
|--------------|--------------------------|
|<span data-ttu-id="3581f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3581f-123">Authorization</span></span> |<span data-ttu-id="3581f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3581f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3581f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3581f-126">Request body</span></span>
<span data-ttu-id="3581f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3581f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3581f-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="3581f-128">Response</span></span>
<span data-ttu-id="3581f-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **ажедаккаунтспайабле** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3581f-129">If successful, this method returns a `200 OK` response code and an **agedAccountsPayable** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3581f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3581f-130">Example</span></span>

<span data-ttu-id="3581f-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="3581f-131">**Request**</span></span>

<span data-ttu-id="3581f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3581f-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/agedAccountsPayable?$filter=periodLengthFilter eq '3M'
```

<span data-ttu-id="3581f-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="3581f-133">**Response**</span></span>

<span data-ttu-id="3581f-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3581f-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="3581f-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3581f-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3581f-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3581f-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "vendorId": "id-value",
  "vendorNumber": "50000",
  "name": "Nod Publishers",
  "currencyCode": "USD",
  "balanceDue": 17273.87,
  "currentAmount": 0,
  "period1Amount": 0,
  "period2Amount": 0,
  "period3Amount": 17273.87,
  "agedAsOfDate": "2019-01-01",
  "periodLengthFilter": "3M"  
}
```
