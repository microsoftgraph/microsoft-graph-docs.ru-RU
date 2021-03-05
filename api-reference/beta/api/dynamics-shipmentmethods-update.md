---
title: Обновление отгрузкиMethods
description: Обновляет объект метода отправки в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 05802c0acda91d56661838aaf0e9fef04d8ba2da
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50474241"
---
# <a name="update-shipmentmethods"></a><span data-ttu-id="104e3-103">Обновление отгрузкиMethods</span><span class="sxs-lookup"><span data-stu-id="104e3-103">Update shipmentMethods</span></span>

<span data-ttu-id="104e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="104e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="104e3-105">Обновление свойств объекта метода отгрузки для Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="104e3-105">Update the properties of a shipment method object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="104e3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="104e3-106">Permissions</span></span>
<span data-ttu-id="104e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="104e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="104e3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="104e3-109">Permission type</span></span> |<span data-ttu-id="104e3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="104e3-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="104e3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="104e3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="104e3-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="104e3-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="104e3-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="104e3-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="104e3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="104e3-114">Not supported.</span></span>|
|<span data-ttu-id="104e3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="104e3-115">Application</span></span>|<span data-ttu-id="104e3-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="104e3-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="104e3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="104e3-117">HTTP request</span></span>
```
PATCH /financials/companies/{id}/shipmentMethods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="104e3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="104e3-118">Optional query parameters</span></span>
<span data-ttu-id="104e3-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="104e3-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="104e3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="104e3-120">Request headers</span></span>
|<span data-ttu-id="104e3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="104e3-121">Header</span></span>|<span data-ttu-id="104e3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="104e3-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="104e3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="104e3-123">Authorization</span></span> |<span data-ttu-id="104e3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="104e3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="104e3-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="104e3-126">Content-Type</span></span>  |<span data-ttu-id="104e3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="104e3-127">application/json</span></span>|
|<span data-ttu-id="104e3-128">If-Match</span><span class="sxs-lookup"><span data-stu-id="104e3-128">If-Match</span></span>      |<span data-ttu-id="104e3-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="104e3-129">Required.</span></span> <span data-ttu-id="104e3-130">Если этот загон запроса включен и предоставленный eTag не совпадает с текущим тегом на **пересылкеMethods,** **отправкаMethods** не будет обновляться.</span><span class="sxs-lookup"><span data-stu-id="104e3-130">When this request header is included and the eTag provided does not match the current tag on the **shipmentMethods**, the **shipmentMethods** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="104e3-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="104e3-131">Request body</span></span>
<span data-ttu-id="104e3-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="104e3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="104e3-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="104e3-135">Response</span></span>
<span data-ttu-id="104e3-136">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` **shipmentMethods** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="104e3-136">If successful, this method returns a `200 OK` response code and an updated **shipmentMethods** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="104e3-137">Пример</span><span class="sxs-lookup"><span data-stu-id="104e3-137">Example</span></span>

<span data-ttu-id="104e3-138">**Запрос**</span><span class="sxs-lookup"><span data-stu-id="104e3-138">**Request**</span></span>

<span data-ttu-id="104e3-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="104e3-139">Here is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/shipmentMethods/{id}
Content-type: application/json

{
  "displayName": "Pickup at Store Location"
}
```

<span data-ttu-id="104e3-140">**Отклик**</span><span class="sxs-lookup"><span data-stu-id="104e3-140">**Response**</span></span>

<span data-ttu-id="104e3-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="104e3-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="104e3-142">**Примечание.** Показанный здесь объект ответа может быть сокращен для читаемости.</span><span class="sxs-lookup"><span data-stu-id="104e3-142">**Note**:  The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="104e3-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="104e3-143">All the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "PICKUP",
  "displayName": "Pickup at Store Location",
  "lastModifiedDateTime": "2017-03-15T02:20:57.09Z"
  }
```



