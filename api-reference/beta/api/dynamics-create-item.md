---
title: Создание элементов
description: Создает объект элемента в Центре бизнеса Dynamics 365.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 27c56da8501ec8617228754327c8c2ad35f2f653
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473296"
---
# <a name="create-items"></a><span data-ttu-id="a1f08-103">Создание элементов</span><span class="sxs-lookup"><span data-stu-id="a1f08-103">Create items</span></span>

<span data-ttu-id="a1f08-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1f08-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1f08-105">Создайте элемент в Dynamics 365 Business Central для использования в счетах, кавычках и т. д.</span><span class="sxs-lookup"><span data-stu-id="a1f08-105">Create an item in Dynamics 365 Business Central for use on invoices, quotes, etc.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1f08-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a1f08-106">Permissions</span></span>
<span data-ttu-id="a1f08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1f08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1f08-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a1f08-109">Permission type</span></span> |<span data-ttu-id="a1f08-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a1f08-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="a1f08-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a1f08-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a1f08-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1f08-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="a1f08-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a1f08-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a1f08-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a1f08-114">Not supported.</span></span>|
|<span data-ttu-id="a1f08-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a1f08-115">Application</span></span>|<span data-ttu-id="a1f08-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1f08-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1f08-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a1f08-117">HTTP request</span></span>
```http
POST /financials/companies/{id}/items
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1f08-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a1f08-118">Optional query parameters</span></span>
<span data-ttu-id="a1f08-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a1f08-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1f08-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a1f08-120">Request headers</span></span>
|<span data-ttu-id="a1f08-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a1f08-121">Header</span></span>       |<span data-ttu-id="a1f08-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a1f08-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="a1f08-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a1f08-123">Authorization</span></span>|<span data-ttu-id="a1f08-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1f08-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a1f08-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a1f08-126">Content-Type</span></span> |<span data-ttu-id="a1f08-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a1f08-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="a1f08-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a1f08-128">Request body</span></span>
<span data-ttu-id="a1f08-129">В теле запроса поставляют представление JSON объекта **элементов.**</span><span class="sxs-lookup"><span data-stu-id="a1f08-129">In the request body, supply a JSON representation of an **items** object.</span></span>

## <a name="response"></a><span data-ttu-id="a1f08-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a1f08-130">Response</span></span>
<span data-ttu-id="a1f08-131">В случае успешной работы этот метод возвращает код ответа и ```201 Created``` объект **элементов** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a1f08-131">If successful, this method returns ```201 Created``` response code and an **items** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1f08-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a1f08-132">Example</span></span>
<span data-ttu-id="a1f08-133">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="a1f08-133">**Request**</span></span>

<span data-ttu-id="a1f08-134">Вот пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a1f08-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/items
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

<span data-ttu-id="a1f08-135">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="a1f08-135">**Response**</span></span>

<span data-ttu-id="a1f08-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a1f08-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="a1f08-137">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a1f08-137">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a1f08-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a1f08-138">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "number": "1896-S",
  "displayName": "ATHENS Desk",
  "lastModifiedDateTime": "2015-11-09T02:14:32Z"
}
```



