---
title: Создание customerPayments
description: Создает объект клиентской оплаты в Dynamics 365 Business Central.
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 6647852d3d48d7f63aab6f2f63140ca474c7043b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473352"
---
# <a name="create-customerpayments"></a><span data-ttu-id="7a45e-103">Создание customerPayments</span><span class="sxs-lookup"><span data-stu-id="7a45e-103">Create customerPayments</span></span>

<span data-ttu-id="7a45e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a45e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a45e-105">Создает объект клиентской оплаты в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="7a45e-105">Creates a customer payment object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a45e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a45e-106">Permissions</span></span>
<span data-ttu-id="7a45e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a45e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a45e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a45e-109">Permission type</span></span> |<span data-ttu-id="7a45e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a45e-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="7a45e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a45e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7a45e-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a45e-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="7a45e-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a45e-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7a45e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a45e-114">Not supported.</span></span>|
|<span data-ttu-id="7a45e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a45e-115">Application</span></span>|<span data-ttu-id="7a45e-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a45e-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a45e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a45e-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7a45e-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7a45e-118">Optional query parameters</span></span>
<span data-ttu-id="7a45e-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7a45e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a45e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a45e-120">Request headers</span></span>
|<span data-ttu-id="7a45e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a45e-121">Header</span></span>        |<span data-ttu-id="7a45e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7a45e-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="7a45e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a45e-123">Authorization</span></span> |<span data-ttu-id="7a45e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a45e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="7a45e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a45e-126">Content-Type</span></span>  |<span data-ttu-id="7a45e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7a45e-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="7a45e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a45e-128">Request body</span></span>
<span data-ttu-id="7a45e-129">В теле запроса поставляем представление JSON объекта **customerPayments.**</span><span class="sxs-lookup"><span data-stu-id="7a45e-129">In the request body, supply a JSON representation of **customerPayments** object.</span></span>

## <a name="response"></a><span data-ttu-id="7a45e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a45e-130">Response</span></span>
<span data-ttu-id="7a45e-131">В случае успешного выполнения этот метод возвращает код ответа и объект ```201 Created``` **customerPayments** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7a45e-131">If successful, this method returns ```201 Created``` response code and a **customerPayments** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a45e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7a45e-132">Example</span></span>

<span data-ttu-id="7a45e-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="7a45e-133">**Request**</span></span>

<span data-ttu-id="7a45e-134">Вот пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a45e-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals/{id}/customerPayments
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
<span data-ttu-id="7a45e-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="7a45e-135">**Response**</span></span>

```http
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



