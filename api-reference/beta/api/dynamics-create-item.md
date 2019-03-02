---
title: Создание элементов
description: Создает объект item в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 68bb1e1c8fbfa3c7675b5ef6dc39de24ffad2ecd
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365838"
---
# <a name="create-items"></a><span data-ttu-id="6b91d-103">Создание элементов</span><span class="sxs-lookup"><span data-stu-id="6b91d-103">Create items</span></span>
<span data-ttu-id="6b91d-104">Создание элемента в Dynamics 365 Business Central для использования в счетах, квотах и т. д.</span><span class="sxs-lookup"><span data-stu-id="6b91d-104">Create an item in Dynamics 365 Business Central for use on invoices, quotes, etc.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b91d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b91d-105">Permissions</span></span>
<span data-ttu-id="6b91d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b91d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b91d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b91d-108">Permission type</span></span> |<span data-ttu-id="6b91d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b91d-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="6b91d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b91d-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6b91d-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b91d-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="6b91d-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b91d-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6b91d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b91d-113">Not supported.</span></span>|
|<span data-ttu-id="6b91d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b91d-114">Application</span></span>|<span data-ttu-id="6b91d-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b91d-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b91d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b91d-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/items
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6b91d-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6b91d-117">Optional query parameters</span></span>
<span data-ttu-id="6b91d-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6b91d-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b91d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b91d-119">Request headers</span></span>
|<span data-ttu-id="6b91d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b91d-120">Header</span></span>       |<span data-ttu-id="6b91d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6b91d-121">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="6b91d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b91d-122">Authorization</span></span>|<span data-ttu-id="6b91d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b91d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6b91d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6b91d-125">Content-Type</span></span> |<span data-ttu-id="6b91d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b91d-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="6b91d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b91d-127">Request body</span></span>
<span data-ttu-id="6b91d-128">В тексте запроса добавьте представление объекта **Items** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b91d-128">In the request body, supply a JSON representation of an **items** object.</span></span>

## <a name="response"></a><span data-ttu-id="6b91d-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b91d-129">Response</span></span>
<span data-ttu-id="6b91d-130">В случае успешного выполнения этот метод ```201 Created``` возвращает код отклика и объект **Items** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6b91d-130">If successful, this method returns ```201 Created``` response code and an **items** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b91d-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6b91d-131">Example</span></span>
<span data-ttu-id="6b91d-132">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="6b91d-132">**Request**</span></span>

<span data-ttu-id="6b91d-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b91d-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/items
Content-type: application/json

{
  "number": "1896-S",
  "displayName": "ATHENS Desk",
  "type": "Inventory",
  "blocked": false,
  "baseUnitOfMeasureId": "65bdbd3a-39f1-49f4-bf24-598cbac36230",
  "gtin": "",
  "itemCategoryId": "5b0b9c1c-312d-4809-96b2-056690a11057",
  "inventory": 0,
  "unitPrice": 1000.8,
  "priceIncludesTax": false,
  "unitCost": 780.7,
  "taxGroupCode": "FURNITURE"
} 

```

<span data-ttu-id="6b91d-134">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="6b91d-134">**Response**</span></span>

<span data-ttu-id="6b91d-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6b91d-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="6b91d-136">**Note**: объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6b91d-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6b91d-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b91d-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "1896-S",
  "displayName": "ATHENS Desk",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z"
}
```

