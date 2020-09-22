---
title: Удаление Кустомерпайментс
description: Удаляет объект платежа клиента в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 1127f996cbe002e9ca1f475dcbafccf0a3a6fded
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981459"
---
# <a name="delete-customerpayments"></a><span data-ttu-id="344ce-103">Удаление Кустомерпайментс</span><span class="sxs-lookup"><span data-stu-id="344ce-103">Delete customerPayments</span></span>

<span data-ttu-id="344ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="344ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="344ce-105">Удаление Кустомерпаймент из Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="344ce-105">Delete a customerPayment from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="344ce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="344ce-106">Permissions</span></span>
<span data-ttu-id="344ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="344ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="344ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="344ce-109">Permission type</span></span> |<span data-ttu-id="344ce-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="344ce-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="344ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="344ce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="344ce-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="344ce-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="344ce-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="344ce-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="344ce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="344ce-114">Not supported.</span></span>|
|<span data-ttu-id="344ce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="344ce-115">Application</span></span>|<span data-ttu-id="344ce-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="344ce-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="344ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="344ce-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="344ce-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="344ce-118">Optional query parameters</span></span>
<span data-ttu-id="344ce-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="344ce-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="344ce-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="344ce-120">Request headers</span></span>
|<span data-ttu-id="344ce-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="344ce-121">Header</span></span>         |<span data-ttu-id="344ce-122">Значение</span><span class="sxs-lookup"><span data-stu-id="344ce-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="344ce-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="344ce-123">Authorization</span></span>  |<span data-ttu-id="344ce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="344ce-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="344ce-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="344ce-126">If-Match</span></span>       |<span data-ttu-id="344ce-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="344ce-127">Required.</span></span> <span data-ttu-id="344ce-128">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **кустомерпайментс**, **кустомерпайментс** не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="344ce-128">When this request header is included and the eTag provided does not match the current tag on the **customerPayments**, the **customerPayments** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="344ce-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="344ce-129">Request body</span></span>

<span data-ttu-id="344ce-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="344ce-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="344ce-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="344ce-131">Response</span></span>

<span data-ttu-id="344ce-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="344ce-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="344ce-134">Пример</span><span class="sxs-lookup"><span data-stu-id="344ce-134">Example</span></span>

<span data-ttu-id="344ce-135">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="344ce-135">**Request**</span></span>

<span data-ttu-id="344ce-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="344ce-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals/{id}/customerPayments/{id}
```

<span data-ttu-id="344ce-137">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="344ce-137">**Response**</span></span> 

<span data-ttu-id="344ce-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="344ce-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```


