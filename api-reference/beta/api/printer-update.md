---
title: Обновление принтера
description: Обновление свойств объекта Printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 5d3c7a87f12a2c26e26c6afe757812245974206a
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896221"
---
# <a name="update-printer"></a><span data-ttu-id="0a4d2-103">Обновление принтера</span><span class="sxs-lookup"><span data-stu-id="0a4d2-103">Update printer</span></span>

<span data-ttu-id="0a4d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a4d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a4d2-105">Обновление свойств объекта [Printer](../resources/printer.md) .</span><span class="sxs-lookup"><span data-stu-id="0a4d2-105">Update the properties of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a4d2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a4d2-106">Permissions</span></span>
<span data-ttu-id="0a4d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a4d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0a4d2-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="0a4d2-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="0a4d2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a4d2-110">Permission type</span></span> | <span data-ttu-id="0a4d2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a4d2-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0a4d2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a4d2-112">Delegated (work or school account)</span></span>| <span data-ttu-id="0a4d2-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="0a4d2-113">Users.Read.All</span></span> |
|<span data-ttu-id="0a4d2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a4d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a4d2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a4d2-115">Not Supported.</span></span>|
|<span data-ttu-id="0a4d2-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="0a4d2-116">Application</span></span>|<span data-ttu-id="0a4d2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a4d2-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a4d2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a4d2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0a4d2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a4d2-119">Request headers</span></span>
| <span data-ttu-id="0a4d2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0a4d2-120">Name</span></span>       | <span data-ttu-id="0a4d2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0a4d2-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0a4d2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a4d2-122">Authorization</span></span> | <span data-ttu-id="0a4d2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a4d2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0a4d2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0a4d2-125">Content-type</span></span>  | <span data-ttu-id="0a4d2-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a4d2-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a4d2-128">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a4d2-128">Request body</span></span>
<span data-ttu-id="0a4d2-129">В тексте запроса укажите значения для соответствующих полей [принтера](../resources/printer.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0a4d2-129">In the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="0a4d2-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="0a4d2-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0a4d2-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0a4d2-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0a4d2-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a4d2-132">Property</span></span>     | <span data-ttu-id="0a4d2-133">Тип</span><span class="sxs-lookup"><span data-stu-id="0a4d2-133">Type</span></span>        | <span data-ttu-id="0a4d2-134">Описание</span><span class="sxs-lookup"><span data-stu-id="0a4d2-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0a4d2-135">location</span><span class="sxs-lookup"><span data-stu-id="0a4d2-135">location</span></span>|[<span data-ttu-id="0a4d2-136">принтерлокатион</span><span class="sxs-lookup"><span data-stu-id="0a4d2-136">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="0a4d2-137">Физическое и/или организационное расположение принтера.</span><span class="sxs-lookup"><span data-stu-id="0a4d2-137">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="0a4d2-138">name</span><span class="sxs-lookup"><span data-stu-id="0a4d2-138">name</span></span>|<span data-ttu-id="0a4d2-139">String</span><span class="sxs-lookup"><span data-stu-id="0a4d2-139">String</span></span>|<span data-ttu-id="0a4d2-140">Имя принтера.</span><span class="sxs-lookup"><span data-stu-id="0a4d2-140">The name of the printer.</span></span>|

## <a name="response"></a><span data-ttu-id="0a4d2-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a4d2-141">Response</span></span>
<span data-ttu-id="0a4d2-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Printer](../resources/printer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0a4d2-142">If successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0a4d2-143">Пример</span><span class="sxs-lookup"><span data-stu-id="0a4d2-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a4d2-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a4d2-144">Request</span></span>
<span data-ttu-id="0a4d2-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a4d2-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printer"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/printers/{id}
Content-type: application/json
Content-length: 124

{
  "name": "PrinterName",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```
##### <a name="response"></a><span data-ttu-id="0a4d2-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a4d2-146">Response</span></span>
<span data-ttu-id="0a4d2-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0a4d2-147">The following is an example of the response.</span></span>
><span data-ttu-id="0a4d2-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a4d2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1313

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "name": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "acceptingJobs": true,
  "registeredBy": {},
  "status": {
    "processingState": "idle",
    "processingStateReasons": [],
    "processingStateDescription": ""
  },
  "defaults": {
    "copiesPerJob":1,
    "documentMimeType": "application/oxps",
    "finishings": ["none"],
    "mediaType": "stationery"
  },
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3,
    "streetAddress": "One Microsoft Way",
    "subUnit": [
        "Main Plaza",
        "Unit 400"
    ],
    "city": "Redmond",
    "postalCode": "98052",
    "countryOrRegion": "USA",
    "site": "Puget Sound",
    "building": "Studio E",
    "floorNumber": 1,
    "floorDescription": "First Floor",
    "roomNumber": 1234,
    "roomDescription": "First floor copy room",
    "organization": [
        "C+AI",
        "Microsoft Graph"
    ],
    "subdivision": [
        "King County",
        "Red West"
    ],
    "stateOrProvince": "Washington"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->