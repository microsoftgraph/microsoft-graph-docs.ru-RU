---
title: Обновление валют
description: Обновляет объект валюты в Центре бизнеса Dynamics 365.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: f7c9c7b5492ebdcf8b41207722285d3b115ce3a3
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471343"
---
# <a name="update-currencies"></a><span data-ttu-id="85f43-103">Обновление валют</span><span class="sxs-lookup"><span data-stu-id="85f43-103">Update currencies</span></span>

<span data-ttu-id="85f43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85f43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85f43-105">Обновление свойств объекта валюты для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="85f43-105">Update the properties of a currency object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="85f43-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85f43-106">Permissions</span></span>
<span data-ttu-id="85f43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85f43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85f43-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85f43-109">Permission type</span></span> |<span data-ttu-id="85f43-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85f43-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="85f43-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85f43-111">Delegated (work or school account)</span></span>|<span data-ttu-id="85f43-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85f43-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="85f43-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85f43-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="85f43-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85f43-114">Not supported.</span></span>|
|<span data-ttu-id="85f43-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85f43-115">Application</span></span>|<span data-ttu-id="85f43-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85f43-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85f43-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85f43-117">HTTP request</span></span>
```
PATCH /financials/companies/{id}/currencies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="85f43-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="85f43-118">Optional query parameters</span></span>
<span data-ttu-id="85f43-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="85f43-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85f43-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85f43-120">Request headers</span></span>
|<span data-ttu-id="85f43-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85f43-121">Header</span></span>       |<span data-ttu-id="85f43-122">Значение</span><span class="sxs-lookup"><span data-stu-id="85f43-122">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="85f43-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85f43-123">Authorization</span></span>|<span data-ttu-id="85f43-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85f43-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="85f43-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85f43-126">Content-Type</span></span> |<span data-ttu-id="85f43-127">application/json</span><span class="sxs-lookup"><span data-stu-id="85f43-127">application/json</span></span>         |
|<span data-ttu-id="85f43-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="85f43-128">If-Match</span></span>     |<span data-ttu-id="85f43-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="85f43-129">Required.</span></span> <span data-ttu-id="85f43-130">Если этот заглавный запрос включен и предоставленный eTag не совпадает  с текущим тегом в валютах, валюты не будут обновляться.</span><span class="sxs-lookup"><span data-stu-id="85f43-130">When this request header is included and the eTag provided does not match the current tag on the **currencies**, the **currencies** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85f43-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85f43-131">Request body</span></span>
<span data-ttu-id="85f43-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="85f43-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="85f43-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="85f43-135">Response</span></span>
<span data-ttu-id="85f43-136">В случае успешной работы этот метод возвращает код ответа и объект обновленных валют `200 OK` в тексте  ответа.</span><span class="sxs-lookup"><span data-stu-id="85f43-136">If successful, this method returns a `200 OK` response code and an updated **currencies** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85f43-137">Пример</span><span class="sxs-lookup"><span data-stu-id="85f43-137">Example</span></span>

<span data-ttu-id="85f43-138">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="85f43-138">**Request**</span></span>

<span data-ttu-id="85f43-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85f43-139">Here is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/currencies/{id}
Content-type: application/json

{
    "displayName": "United States Dollar"
}
```

<span data-ttu-id="85f43-140">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="85f43-140">**Response**</span></span>

<span data-ttu-id="85f43-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="85f43-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="85f43-142">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="85f43-142">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="85f43-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85f43-143">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "US",
  "displayName": "United States Dollar",
  "symbol": "$",
  "amountDecimalPlaces": "2:2",
  "amountRoundingPrecision": 0.01,
  "lastModifiedDateTime": "2017-03-22T21:12:18.793Z"
}
```


