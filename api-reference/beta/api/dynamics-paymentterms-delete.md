---
title: Удаление Пайменттермс
description: Удаляет объект термина платежа в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 515086b79c6a75c75375d159ef20eb2cc56ef231
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008248"
---
# <a name="delete-paymentterms"></a><span data-ttu-id="9ea36-103">Удаление Пайменттермс</span><span class="sxs-lookup"><span data-stu-id="9ea36-103">Delete paymentTerms</span></span>

<span data-ttu-id="9ea36-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ea36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ea36-105">Удаление объекта условий оплаты из Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="9ea36-105">Delete a payment terms object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ea36-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ea36-106">Permissions</span></span>
<span data-ttu-id="9ea36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ea36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ea36-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ea36-109">Permission type</span></span> |<span data-ttu-id="9ea36-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ea36-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="9ea36-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ea36-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9ea36-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ea36-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="9ea36-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ea36-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9ea36-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ea36-114">Not supported.</span></span>|
|<span data-ttu-id="9ea36-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="9ea36-115">Application</span></span>|<span data-ttu-id="9ea36-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ea36-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ea36-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ea36-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/paymentTerms/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ea36-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9ea36-118">Optional query parameters</span></span>
<span data-ttu-id="9ea36-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9ea36-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ea36-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ea36-120">Request headers</span></span>

|<span data-ttu-id="9ea36-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ea36-121">Header</span></span>         |<span data-ttu-id="9ea36-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9ea36-122">Value</span></span>                     |
|---------------|--------------------------|
|<span data-ttu-id="9ea36-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ea36-123">Authorization</span></span>  |<span data-ttu-id="9ea36-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ea36-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="9ea36-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="9ea36-126">If-Match</span></span>       |<span data-ttu-id="9ea36-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9ea36-127">Required.</span></span> <span data-ttu-id="9ea36-128">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **пайменттермс**, **пайменттермс** не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="9ea36-128">When this request header is included and the eTag provided does not match the current tag on the **paymentTerms**, the **paymentTerms** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ea36-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ea36-129">Request body</span></span>
<span data-ttu-id="9ea36-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ea36-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ea36-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ea36-131">Response</span></span>
<span data-ttu-id="9ea36-p104">В случае успешного выполнения этот метод возвращает код отклика ```204 No Content```. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9ea36-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ea36-134">Пример</span><span class="sxs-lookup"><span data-stu-id="9ea36-134">Example</span></span>

<span data-ttu-id="9ea36-135">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="9ea36-135">**Request**</span></span>

<span data-ttu-id="9ea36-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ea36-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/paymentTerms/{id}
```

<span data-ttu-id="9ea36-137">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="9ea36-137">**Response**</span></span> 

<span data-ttu-id="9ea36-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9ea36-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```


