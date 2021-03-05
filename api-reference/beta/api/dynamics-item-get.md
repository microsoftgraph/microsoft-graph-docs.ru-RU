---
title: Получение элементов
description: Получает объект элемента в Центре бизнеса Dynamics 365.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: efcb64327462f69aba4948938d1f6763912866e2
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471266"
---
# <a name="get-items"></a><span data-ttu-id="a89ea-103">Получение элементов</span><span class="sxs-lookup"><span data-stu-id="a89ea-103">Get items</span></span>

<span data-ttu-id="a89ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a89ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a89ea-105">Извлечение свойств и связей объекта элемента для Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="a89ea-105">Retrieve the properties and relationships of an item object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="a89ea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a89ea-106">Permissions</span></span>
<span data-ttu-id="a89ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a89ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a89ea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a89ea-109">Permission type</span></span> |<span data-ttu-id="a89ea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a89ea-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a89ea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a89ea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a89ea-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a89ea-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a89ea-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a89ea-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a89ea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a89ea-114">Not supported.</span></span>|
|<span data-ttu-id="a89ea-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a89ea-115">Application</span></span>|<span data-ttu-id="a89ea-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a89ea-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a89ea-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a89ea-117">HTTP request</span></span>

```
GET /financials/companies/{id}/items/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a89ea-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a89ea-118">Optional query parameters</span></span>
<span data-ttu-id="a89ea-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a89ea-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a89ea-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a89ea-120">Request headers</span></span>
|<span data-ttu-id="a89ea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a89ea-121">Header</span></span>       |<span data-ttu-id="a89ea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a89ea-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="a89ea-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a89ea-123">Authorization</span></span>|<span data-ttu-id="a89ea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a89ea-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a89ea-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a89ea-126">Request body</span></span>
<span data-ttu-id="a89ea-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a89ea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a89ea-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a89ea-128">Response</span></span>
<span data-ttu-id="a89ea-129">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект **элементов** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a89ea-129">If successful, this method returns a `200 OK` response code and an **items** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a89ea-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a89ea-130">Example</span></span>
<span data-ttu-id="a89ea-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="a89ea-131">**Request**</span></span>

<span data-ttu-id="a89ea-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a89ea-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/items/{id}
```

<span data-ttu-id="a89ea-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="a89ea-133">**Response**</span></span>

<span data-ttu-id="a89ea-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a89ea-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="a89ea-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a89ea-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a89ea-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a89ea-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "number": "1896-S",
  "displayName": "ATHENS Desk",
  "type": "Inventory",
  "blocked": false,
  "baseUnitOfMeasureId": "id-value",
  "gtin": "",
  "itemCategoryId": "id-value"
  "inventory": 0,
  "unitPrice": 1000.8,
  "priceIncludesTax": false,
  "unitCost": 780.7,
  "taxGroupId": "id-value",
  "taxGroupCode": "FURNITURE",
  "lastModifiedDateTime": "2017-03-07T00:35:30.073Z"
}

```



