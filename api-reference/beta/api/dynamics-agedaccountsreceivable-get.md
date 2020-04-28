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
ms.openlocfilehash: 70b0e5824f29c356a1df3c74e33a3fed355bd166
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431979"
---
# <a name="get-agedaccountsreceivable"></a><span data-ttu-id="b391e-103">Получение Ажедаккаунтсрецеивабле</span><span class="sxs-lookup"><span data-stu-id="b391e-103">Get agedAccountsReceivable</span></span>

<span data-ttu-id="b391e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b391e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b391e-105">Получение свойств и связей для устаревших объектов отчета о расчетах с поставщиками для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="b391e-105">Retrieve the properties and relationships of an aged accounts receivable report object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="b391e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b391e-106">Permissions</span></span>
<span data-ttu-id="b391e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b391e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b391e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b391e-109">Permission type</span></span> |<span data-ttu-id="b391e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b391e-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="b391e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b391e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b391e-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b391e-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="b391e-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b391e-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b391e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b391e-114">Not supported.</span></span>|
|<span data-ttu-id="b391e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b391e-115">Application</span></span>|<span data-ttu-id="b391e-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b391e-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b391e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b391e-117">HTTP request</span></span>
```
GET /financials/companies/{id}/agedAccountsReceivable
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b391e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b391e-118">Optional query parameters</span></span>
<span data-ttu-id="b391e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b391e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b391e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b391e-120">Request headers</span></span>
|<span data-ttu-id="b391e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b391e-121">Header</span></span>|<span data-ttu-id="b391e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b391e-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="b391e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b391e-123">Authorization</span></span>  |<span data-ttu-id="b391e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b391e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b391e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b391e-126">Request body</span></span>
<span data-ttu-id="b391e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b391e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b391e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b391e-128">Response</span></span>
<span data-ttu-id="b391e-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **ажедаккаунтсрецеивабле** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b391e-129">If successful, this method returns a `200 OK` response code and an **agedAccountsReceivable** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b391e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b391e-130">Example</span></span>

<span data-ttu-id="b391e-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="b391e-131">**Request**</span></span>

<span data-ttu-id="b391e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b391e-132">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/agedAccountsReceivable?$filter=periodLengthFilter eq '3M'
```

<span data-ttu-id="b391e-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="b391e-133">**Response**</span></span>

<span data-ttu-id="b391e-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b391e-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="b391e-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b391e-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b391e-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b391e-136">All the properties will be returned from an actual call.</span></span>

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
