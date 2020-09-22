---
title: Обновление Унитсофмеасуре
description: Обновляет объект единицы измерения в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: d464d2e45939c1956e2fce981328fff0484195c5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008076"
---
# <a name="update-unitsofmeasure"></a><span data-ttu-id="7678f-103">Обновление Унитсофмеасуре</span><span class="sxs-lookup"><span data-stu-id="7678f-103">Update unitsOfMeasure</span></span>

<span data-ttu-id="7678f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7678f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7678f-105">Обновление свойств объекта Units of Measure для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="7678f-105">Update the properties of a units of measure object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="7678f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7678f-106">Permissions</span></span>
<span data-ttu-id="7678f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7678f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7678f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7678f-109">Permission type</span></span> |<span data-ttu-id="7678f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7678f-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="7678f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7678f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7678f-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7678f-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="7678f-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7678f-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7678f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7678f-114">Not supported.</span></span>|
|<span data-ttu-id="7678f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7678f-115">Application</span></span>|<span data-ttu-id="7678f-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7678f-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7678f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7678f-117">HTTP request</span></span>

```
PATCH /financials/companies/{id}/unitsOfMeasure/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7678f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7678f-118">Optional query parameters</span></span>
<span data-ttu-id="7678f-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7678f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7678f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7678f-120">Request headers</span></span>
|<span data-ttu-id="7678f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7678f-121">Header</span></span>|<span data-ttu-id="7678f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7678f-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="7678f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7678f-123">Authorization</span></span> |<span data-ttu-id="7678f-124">Носителя.</span><span class="sxs-lookup"><span data-stu-id="7678f-124">Bearer.</span></span> <span data-ttu-id="7678f-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7678f-125">Required.</span></span>|
|<span data-ttu-id="7678f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7678f-126">Content-Type</span></span>  |<span data-ttu-id="7678f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7678f-127">application/json</span></span>|
|<span data-ttu-id="7678f-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="7678f-128">If-Match</span></span>      |<span data-ttu-id="7678f-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7678f-129">Required.</span></span> <span data-ttu-id="7678f-130">Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **унитсофмеасуре**, **унитсофмеасуре** не будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="7678f-130">When this request header is included and the eTag provided does not match the current tag on the **unitsOfMeasure**, the **unitsOfMeasure** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7678f-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7678f-131">Request body</span></span>
<span data-ttu-id="7678f-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7678f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="7678f-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="7678f-135">Response</span></span>
<span data-ttu-id="7678f-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект **унитсофмеасуре** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7678f-136">If successful, this method returns a `200 OK` response code and an updated **unitsOfMeasure** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7678f-137">Пример</span><span class="sxs-lookup"><span data-stu-id="7678f-137">Example</span></span>

<span data-ttu-id="7678f-138">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="7678f-138">**Request**</span></span>

<span data-ttu-id="7678f-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7678f-139">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/unitsOfMeasure/{id}
Content-type: application/json

{
  "displayName": "One Piece"
}
```

<span data-ttu-id="7678f-140">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="7678f-140">**Response**</span></span>

<span data-ttu-id="7678f-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7678f-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="7678f-142">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7678f-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7678f-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7678f-143">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "PCS",
  "displayName": "One Piece",
  "internationalStandardCode": "EA",
  "lastModifiedDateTime": "2017-03-15T01:21:09.563Z"
}
```



