---
title: Обновление customerPayments
description: Обновляет объект клиентской оплаты в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: e67ed716ae8d92bc4e1d7218d5cddebb7e89bfcf
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471299"
---
# <a name="update-customerpayments"></a><span data-ttu-id="9ec49-103">Обновление customerPayments</span><span class="sxs-lookup"><span data-stu-id="9ec49-103">Update customerPayments</span></span>

<span data-ttu-id="9ec49-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ec49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ec49-105">Обновление свойств объекта платежей клиента для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="9ec49-105">Update the properties of a customer payment object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ec49-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ec49-106">Permissions</span></span>
<span data-ttu-id="9ec49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ec49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ec49-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ec49-109">Permission type</span></span> |<span data-ttu-id="9ec49-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ec49-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="9ec49-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ec49-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9ec49-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ec49-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="9ec49-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ec49-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9ec49-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ec49-114">Not supported.</span></span>|
|<span data-ttu-id="9ec49-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ec49-115">Application</span></span>|<span data-ttu-id="9ec49-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ec49-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ec49-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ec49-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ec49-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9ec49-118">Optional query parameters</span></span>
<span data-ttu-id="9ec49-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9ec49-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ec49-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ec49-120">Request headers</span></span>
|<span data-ttu-id="9ec49-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ec49-121">Header</span></span>        |<span data-ttu-id="9ec49-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9ec49-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="9ec49-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ec49-123">Authorization</span></span> |<span data-ttu-id="9ec49-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ec49-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9ec49-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9ec49-126">Content-Type</span></span>  |<span data-ttu-id="9ec49-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9ec49-127">application/json</span></span>         |
|<span data-ttu-id="9ec49-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="9ec49-128">If-Match</span></span>      |<span data-ttu-id="9ec49-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9ec49-129">Required.</span></span> <span data-ttu-id="9ec49-130">Если заглавная информация об этом запросе включена и предоставленный eTag не соответствует текущему тегу на **customerPayments,** **клиенты** не будут обновляться.</span><span class="sxs-lookup"><span data-stu-id="9ec49-130">When this request header is included and the eTag provided does not match the current tag on the **customerPayments**, the **customerPayments** will not be updated.</span></span>    |

## <a name="request-body"></a><span data-ttu-id="9ec49-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ec49-131">Request body</span></span>
<span data-ttu-id="9ec49-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9ec49-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="9ec49-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ec49-135">Response</span></span>
<span data-ttu-id="9ec49-136">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` **customerPayments** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9ec49-136">If successful, this method returns a `200 OK` response code and an updated **customerPayments** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ec49-137">Пример</span><span class="sxs-lookup"><span data-stu-id="9ec49-137">Example</span></span>

<span data-ttu-id="9ec49-138">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="9ec49-138">**Request**</span></span>

<span data-ttu-id="9ec49-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ec49-139">Here is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
Content-type: application/json

{
  "amount": 2000
}
```

<span data-ttu-id="9ec49-140">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="9ec49-140">**Response**</span></span>

<span data-ttu-id="9ec49-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9ec49-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="9ec49-142">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9ec49-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9ec49-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ec49-143">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "customerId": "customerId-value",
  "customerNumber": "",
  "contactId": "contactId-value",
  "postingDate": "2015-12-31",
  "documentNumber": "D00001",
  "externalDocumentNumber": "",
  "amount": -2000,
  "appliesToInvoiceId": "appliesToInvoiceId-value",
  "appliesToInvoiceNumber": "100000",
  "description": "",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```



