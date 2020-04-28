---
title: Получение Кустомерпайментс
description: Получает объект платежа клиента в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 8a8ea120b0d2422937d0193f181fe80c5c123e7a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42430611"
---
# <a name="get-customerpayments"></a><span data-ttu-id="18d7a-103">Получение Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="18d7a-103">Get customerPayments</span></span>

<span data-ttu-id="18d7a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18d7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18d7a-105">Получение свойств и связей объекта клиентского платежа для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="18d7a-105">Retrieve the properties and relationships of a customer payment object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="18d7a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18d7a-106">Permissions</span></span>
<span data-ttu-id="18d7a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18d7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18d7a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18d7a-109">Permission type</span></span> |<span data-ttu-id="18d7a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18d7a-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="18d7a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18d7a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="18d7a-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18d7a-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="18d7a-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18d7a-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="18d7a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18d7a-114">Not supported.</span></span>|
|<span data-ttu-id="18d7a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18d7a-115">Application</span></span>|<span data-ttu-id="18d7a-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18d7a-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18d7a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18d7a-117">HTTP request</span></span>

```
GET /financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18d7a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="18d7a-118">Optional query parameters</span></span>
<span data-ttu-id="18d7a-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="18d7a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18d7a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18d7a-120">Request headers</span></span>
|<span data-ttu-id="18d7a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18d7a-121">Header</span></span>|<span data-ttu-id="18d7a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="18d7a-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="18d7a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18d7a-123">Authorization</span></span>  |<span data-ttu-id="18d7a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18d7a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18d7a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="18d7a-126">Request body</span></span>
<span data-ttu-id="18d7a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18d7a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18d7a-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="18d7a-128">Response</span></span>
<span data-ttu-id="18d7a-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект **кустомерпайментс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18d7a-129">If successful, this method returns a `200 OK` response code and a **customerPayments** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18d7a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="18d7a-130">Example</span></span>

<span data-ttu-id="18d7a-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="18d7a-131">**Request**</span></span>

<span data-ttu-id="18d7a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18d7a-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
```

<span data-ttu-id="18d7a-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="18d7a-133">**Response**</span></span>

<span data-ttu-id="18d7a-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="18d7a-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="18d7a-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="18d7a-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="18d7a-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18d7a-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "journalDisplayName": "GENERAL",
  "lineNumber": 10000,
  "customerId": "customerId-value",
  "customerNumber": "10400",
  "contactId": "string",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "appliesToInvoiceId": "appliesToInvoiceId-value",
  "appliesToInvoiceNumber": "100000",
  "description": "",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```

