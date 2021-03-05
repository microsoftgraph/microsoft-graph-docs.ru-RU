---
title: Get unitsOfMeasure
description: Получает единицу объекта измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: d907b0bbb2f1cafcc3b6dfbdc03d1b9e27431847
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474136"
---
# <a name="get-unitsofmeasure"></a><span data-ttu-id="d1875-103">Get unitsOfMeasure</span><span class="sxs-lookup"><span data-stu-id="d1875-103">Get unitsOfMeasure</span></span>

<span data-ttu-id="d1875-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1875-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1875-105">Извлечение свойств и связей объекта измерения для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="d1875-105">Retrieve the properties and relationships of a units of measure object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1875-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1875-106">Permissions</span></span>
<span data-ttu-id="d1875-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1875-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1875-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1875-109">Permission type</span></span> |<span data-ttu-id="d1875-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1875-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="d1875-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1875-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d1875-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1875-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="d1875-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1875-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="d1875-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1875-114">Not supported.</span></span>|
|<span data-ttu-id="d1875-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1875-115">Application</span></span>|<span data-ttu-id="d1875-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1875-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1875-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1875-117">HTTP request</span></span>

```
GET /financials/companies/{id}/unitsOfMeasure/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1875-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d1875-118">Optional query parameters</span></span>
<span data-ttu-id="d1875-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d1875-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1875-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1875-120">Request headers</span></span>
|<span data-ttu-id="d1875-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d1875-121">Header</span></span>|<span data-ttu-id="d1875-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d1875-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="d1875-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1875-123">Authorization</span></span>  |<span data-ttu-id="d1875-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1875-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1875-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1875-126">Request body</span></span>
<span data-ttu-id="d1875-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1875-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1875-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1875-128">Response</span></span>
<span data-ttu-id="d1875-129">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` **unitsOfMeasure** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d1875-129">If successful, this method returns a `200 OK` response code and a **unitsOfMeasure** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1875-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d1875-130">Example</span></span>

<span data-ttu-id="d1875-131">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="d1875-131">**Request**</span></span>

<span data-ttu-id="d1875-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d1875-132">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/financials/companies/{id}/unitsOfMeasure/{id}
```

<span data-ttu-id="d1875-133">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="d1875-133">**Response**</span></span>

<span data-ttu-id="d1875-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d1875-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="d1875-135">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d1875-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d1875-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1875-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "PCS",
  "displayName": "Piece",
  "internationalStandardCode": "EA",
  "lastModifiedDateTime": "2017-03-15T01:21:09.563Z"
}
```


