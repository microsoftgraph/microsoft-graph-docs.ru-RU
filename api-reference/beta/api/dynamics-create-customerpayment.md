---
title: Создание Кустомерпайментс
description: Создает объект платежа клиента в Dynamics 365 Business Central.
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 613ad01feddc87941a6e6775195364e75ca4e57a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431678"
---
# <a name="create-customerpayments"></a><span data-ttu-id="81bf9-103">Создание Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="81bf9-103">Create customerPayments</span></span>

<span data-ttu-id="81bf9-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="81bf9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81bf9-105">Создает объект платежа клиента в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="81bf9-105">Creates a customer payment object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="81bf9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81bf9-106">Permissions</span></span>
<span data-ttu-id="81bf9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81bf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81bf9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81bf9-109">Permission type</span></span> |<span data-ttu-id="81bf9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81bf9-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="81bf9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81bf9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="81bf9-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81bf9-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="81bf9-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81bf9-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="81bf9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81bf9-114">Not supported.</span></span>|
|<span data-ttu-id="81bf9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81bf9-115">Application</span></span>|<span data-ttu-id="81bf9-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81bf9-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81bf9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81bf9-117">HTTP request</span></span>
```
POST /financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81bf9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="81bf9-118">Optional query parameters</span></span>
<span data-ttu-id="81bf9-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="81bf9-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81bf9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81bf9-120">Request headers</span></span>
|<span data-ttu-id="81bf9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="81bf9-121">Header</span></span>        |<span data-ttu-id="81bf9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="81bf9-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="81bf9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81bf9-123">Authorization</span></span> |<span data-ttu-id="81bf9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="81bf9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="81bf9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="81bf9-126">Content-Type</span></span>  |<span data-ttu-id="81bf9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="81bf9-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="81bf9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="81bf9-128">Request body</span></span>
<span data-ttu-id="81bf9-129">В тексте запроса добавьте представление объекта **кустомерпайментс** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81bf9-129">In the request body, supply a JSON representation of **customerPayments** object.</span></span>

## <a name="response"></a><span data-ttu-id="81bf9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="81bf9-130">Response</span></span>
<span data-ttu-id="81bf9-131">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **кустомерпайментс** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="81bf9-131">If successful, this method returns ```201 Created``` response code and a **customerPayments** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81bf9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="81bf9-132">Example</span></span>

<span data-ttu-id="81bf9-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="81bf9-133">**Request**</span></span>

<span data-ttu-id="81bf9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81bf9-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournal/{id}/customerPayments
Content-type: application/json

{
  "lineNumber": 10000,
  "customerId": "customerId-value",
  "customerNumber": "10400",
  "contactId": "contactId-value",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": -1500,
  "appliesToInvoiceId": "appliesToInvoiceId-value",
  "appliesToInvoiceNumber": "100000",
  "description": "",
  "comment": "",
}
```
<span data-ttu-id="81bf9-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="81bf9-135">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "customerId": "customerId-value",
  "customerNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "appliesToInvoiceId": "appliesToInvoiceId-value",
  "appliesToInvoiceNumber": "100000",
  "description": "Accounts Receivable",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```

