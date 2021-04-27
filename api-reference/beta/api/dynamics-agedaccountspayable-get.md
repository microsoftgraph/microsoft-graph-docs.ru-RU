---
title: Get agedAccountsPayable
description: Получает объект для оплаты по возрастным счетам в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 717b2df6664ae712f2d9e4c273eac13abf88a930
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046183"
---
# <a name="get-agedaccountspayable"></a><span data-ttu-id="67804-103">Get agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="67804-103">Get agedAccountsPayable</span></span>

<span data-ttu-id="67804-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67804-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67804-105">Извлечение свойств и связей объекта отчетов по возрасту для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="67804-105">Retrieve the properties and relationships of an aged accounts payable report object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="67804-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67804-106">Permissions</span></span>
<span data-ttu-id="67804-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67804-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67804-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67804-109">Permission type</span></span> |<span data-ttu-id="67804-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67804-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="67804-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67804-111">Delegated (work or school account)</span></span>|<span data-ttu-id="67804-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67804-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="67804-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67804-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="67804-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67804-114">Not supported.</span></span>|
|<span data-ttu-id="67804-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67804-115">Application</span></span>|<span data-ttu-id="67804-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67804-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67804-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67804-117">HTTP request</span></span>
```http
GET /financials/companies/{id}/agedAccountsPayable
```
## <a name="optional-query-parameters"></a><span data-ttu-id="67804-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="67804-118">Optional query parameters</span></span>
<span data-ttu-id="67804-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="67804-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67804-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67804-120">Request headers</span></span>
|<span data-ttu-id="67804-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="67804-121">Header</span></span>        |<span data-ttu-id="67804-122">Значение</span><span class="sxs-lookup"><span data-stu-id="67804-122">Value</span></span>                     |
|--------------|--------------------------|
|<span data-ttu-id="67804-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67804-123">Authorization</span></span> |<span data-ttu-id="67804-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67804-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67804-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67804-126">Request body</span></span>
<span data-ttu-id="67804-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="67804-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67804-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="67804-128">Response</span></span>
<span data-ttu-id="67804-129">В случае успешной работы этот метод возвращает код ответа и `200 OK` **объект agedAccountsPayable** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="67804-129">If successful, this method returns a `200 OK` response code and an **agedAccountsPayable** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67804-130">Пример</span><span class="sxs-lookup"><span data-stu-id="67804-130">Example</span></span>

<span data-ttu-id="67804-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="67804-131">**Request**</span></span>

<span data-ttu-id="67804-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67804-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/agedAccountsPayable?$filter=periodLengthFilter eq '3M'
```

<span data-ttu-id="67804-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="67804-133">**Response**</span></span>

<span data-ttu-id="67804-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="67804-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="67804-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="67804-135">**Note**: The response object shown here might be shortened for readability.</span></span>

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


