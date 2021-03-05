---
title: Get customerPayments
description: Получает объект платежей клиента в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 8a84aaf47f96da3eebdcad830846eb3cfc81b52a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471308"
---
# <a name="get-customerpayments"></a><span data-ttu-id="97d94-103">Get customerPayments</span><span class="sxs-lookup"><span data-stu-id="97d94-103">Get customerPayments</span></span>

<span data-ttu-id="97d94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97d94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97d94-105">Извлечение свойств и связей объекта оплаты клиента для Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="97d94-105">Retrieve the properties and relationships of a customer payment object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="97d94-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97d94-106">Permissions</span></span>
<span data-ttu-id="97d94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97d94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97d94-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97d94-109">Permission type</span></span> |<span data-ttu-id="97d94-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97d94-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="97d94-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97d94-111">Delegated (work or school account)</span></span>|<span data-ttu-id="97d94-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97d94-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="97d94-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97d94-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="97d94-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97d94-114">Not supported.</span></span>|
|<span data-ttu-id="97d94-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97d94-115">Application</span></span>|<span data-ttu-id="97d94-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97d94-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97d94-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97d94-117">HTTP request</span></span>

```
GET /financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="97d94-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="97d94-118">Optional query parameters</span></span>
<span data-ttu-id="97d94-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="97d94-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97d94-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97d94-120">Request headers</span></span>
|<span data-ttu-id="97d94-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97d94-121">Header</span></span>|<span data-ttu-id="97d94-122">Значение</span><span class="sxs-lookup"><span data-stu-id="97d94-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="97d94-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97d94-123">Authorization</span></span>  |<span data-ttu-id="97d94-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97d94-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97d94-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97d94-126">Request body</span></span>
<span data-ttu-id="97d94-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97d94-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97d94-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="97d94-128">Response</span></span>
<span data-ttu-id="97d94-129">В случае успешного выполнения этот метод возвращает код отклика и объект `200 OK` **customerPayments** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="97d94-129">If successful, this method returns a `200 OK` response code and a **customerPayments** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97d94-130">Пример</span><span class="sxs-lookup"><span data-stu-id="97d94-130">Example</span></span>

<span data-ttu-id="97d94-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="97d94-131">**Request**</span></span>

<span data-ttu-id="97d94-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97d94-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
```

<span data-ttu-id="97d94-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="97d94-133">**Response**</span></span>

<span data-ttu-id="97d94-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="97d94-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="97d94-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="97d94-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="97d94-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97d94-136">All the properties will be returned from an actual call.</span></span>

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



