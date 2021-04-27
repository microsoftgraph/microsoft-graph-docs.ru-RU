---
title: Получение элементов
description: Получает объект элемента в Центре бизнеса Dynamics 365.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 24765baa81ead30b349ac3a560ef6b06a99f2d35
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52045324"
---
# <a name="get-items"></a><span data-ttu-id="57dcb-103">Получение элементов</span><span class="sxs-lookup"><span data-stu-id="57dcb-103">Get items</span></span>

<span data-ttu-id="57dcb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57dcb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57dcb-105">Извлечение свойств и связей объекта элемента для Центра бизнеса Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="57dcb-105">Retrieve the properties and relationships of an item object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="57dcb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57dcb-106">Permissions</span></span>
<span data-ttu-id="57dcb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57dcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57dcb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57dcb-109">Permission type</span></span> |<span data-ttu-id="57dcb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57dcb-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="57dcb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57dcb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="57dcb-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57dcb-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="57dcb-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57dcb-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="57dcb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57dcb-114">Not supported.</span></span>|
|<span data-ttu-id="57dcb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57dcb-115">Application</span></span>|<span data-ttu-id="57dcb-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57dcb-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57dcb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57dcb-117">HTTP request</span></span>

```
GET /financials/companies/{id}/items/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57dcb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="57dcb-118">Optional query parameters</span></span>
<span data-ttu-id="57dcb-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="57dcb-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57dcb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57dcb-120">Request headers</span></span>
|<span data-ttu-id="57dcb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57dcb-121">Header</span></span>       |<span data-ttu-id="57dcb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="57dcb-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="57dcb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57dcb-123">Authorization</span></span>|<span data-ttu-id="57dcb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57dcb-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="57dcb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57dcb-126">Request body</span></span>
<span data-ttu-id="57dcb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57dcb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57dcb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="57dcb-128">Response</span></span>
<span data-ttu-id="57dcb-129">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект **элементов** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="57dcb-129">If successful, this method returns a `200 OK` response code and an **items** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57dcb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="57dcb-130">Example</span></span>
<span data-ttu-id="57dcb-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="57dcb-131">**Request**</span></span>

<span data-ttu-id="57dcb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57dcb-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/items/{id}
```

<span data-ttu-id="57dcb-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="57dcb-133">**Response**</span></span>

<span data-ttu-id="57dcb-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="57dcb-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="57dcb-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="57dcb-135">**Note**: The response object shown here might be shortened for readability.</span></span>

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



