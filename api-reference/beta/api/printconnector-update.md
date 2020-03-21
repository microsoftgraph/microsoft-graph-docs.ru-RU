---
title: Обновление Принтконнектор
description: Обновление свойств объекта Принтконнектор.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 6546693f0a158de15c6ccb2ca82829748926f16c
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896305"
---
# <a name="update-printconnector"></a><span data-ttu-id="adcdd-103">Обновление Принтконнектор</span><span class="sxs-lookup"><span data-stu-id="adcdd-103">Update printConnector</span></span>

<span data-ttu-id="adcdd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adcdd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adcdd-105">Обновление свойств объекта **принтконнектор** .</span><span class="sxs-lookup"><span data-stu-id="adcdd-105">Update the properties of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="adcdd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="adcdd-106">Permissions</span></span>
<span data-ttu-id="adcdd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adcdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="adcdd-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="adcdd-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="adcdd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="adcdd-110">Permission type</span></span> | <span data-ttu-id="adcdd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="adcdd-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="adcdd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="adcdd-112">Delegated (work or school account)</span></span>| <span data-ttu-id="adcdd-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="adcdd-113">Users.Read.All</span></span> |
|<span data-ttu-id="adcdd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="adcdd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adcdd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adcdd-115">Not Supported.</span></span>|
|<span data-ttu-id="adcdd-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="adcdd-116">Application</span></span>|<span data-ttu-id="adcdd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adcdd-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="adcdd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="adcdd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="adcdd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="adcdd-119">Request headers</span></span>
| <span data-ttu-id="adcdd-120">Имя</span><span class="sxs-lookup"><span data-stu-id="adcdd-120">Name</span></span>       | <span data-ttu-id="adcdd-121">Описание</span><span class="sxs-lookup"><span data-stu-id="adcdd-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="adcdd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="adcdd-122">Authorization</span></span> | <span data-ttu-id="adcdd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="adcdd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="adcdd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="adcdd-125">Content-type</span></span>  | <span data-ttu-id="adcdd-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="adcdd-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="adcdd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="adcdd-128">Request body</span></span>
<span data-ttu-id="adcdd-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="adcdd-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="adcdd-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="adcdd-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="adcdd-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="adcdd-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="adcdd-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="adcdd-132">Property</span></span>     | <span data-ttu-id="adcdd-133">Тип</span><span class="sxs-lookup"><span data-stu-id="adcdd-133">Type</span></span>        | <span data-ttu-id="adcdd-134">Описание</span><span class="sxs-lookup"><span data-stu-id="adcdd-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="adcdd-135">name</span><span class="sxs-lookup"><span data-stu-id="adcdd-135">name</span></span>|<span data-ttu-id="adcdd-136">String</span><span class="sxs-lookup"><span data-stu-id="adcdd-136">String</span></span>|<span data-ttu-id="adcdd-137">Имя соединителя.</span><span class="sxs-lookup"><span data-stu-id="adcdd-137">The name of the connector.</span></span>|
|<span data-ttu-id="adcdd-138">fullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="adcdd-138">fullyQualifiedDomainName</span></span>|<span data-ttu-id="adcdd-139">String</span><span class="sxs-lookup"><span data-stu-id="adcdd-139">String</span></span>|<span data-ttu-id="adcdd-140">Имя узла для соединителя.</span><span class="sxs-lookup"><span data-stu-id="adcdd-140">The connector machine's hostname.</span></span>|
|<span data-ttu-id="adcdd-141">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="adcdd-141">operatingSystem</span></span>|<span data-ttu-id="adcdd-142">String</span><span class="sxs-lookup"><span data-stu-id="adcdd-142">String</span></span>|<span data-ttu-id="adcdd-143">Версия операционной системы на соединителе компьютера.</span><span class="sxs-lookup"><span data-stu-id="adcdd-143">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="adcdd-144">аппверсион</span><span class="sxs-lookup"><span data-stu-id="adcdd-144">appVersion</span></span>|<span data-ttu-id="adcdd-145">String</span><span class="sxs-lookup"><span data-stu-id="adcdd-145">String</span></span>|<span data-ttu-id="adcdd-146">Версия соединителя.</span><span class="sxs-lookup"><span data-stu-id="adcdd-146">The connector's version.</span></span>|
|<span data-ttu-id="adcdd-147">location</span><span class="sxs-lookup"><span data-stu-id="adcdd-147">location</span></span>|[<span data-ttu-id="adcdd-148">принтерлокатион</span><span class="sxs-lookup"><span data-stu-id="adcdd-148">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="adcdd-149">Физическое и/или организационное расположение соединителя.</span><span class="sxs-lookup"><span data-stu-id="adcdd-149">The physical and/or organizational location of the connector.</span></span>|

## <a name="response"></a><span data-ttu-id="adcdd-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="adcdd-150">Response</span></span>
<span data-ttu-id="adcdd-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [принтконнектор](../resources/printConnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="adcdd-151">If successful, this method returns a `200 OK` response code and an updated [printConnector](../resources/printConnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="adcdd-152">Пример</span><span class="sxs-lookup"><span data-stu-id="adcdd-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="adcdd-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="adcdd-153">Request</span></span>
<span data-ttu-id="adcdd-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adcdd-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_connector"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/connectors/{id}
Content-type: application/json
Content-length: 300

{
  "name": "ConnectorName",
  "fullyQualifiedDomainName": "CONNECTOR-MACHINE",
  "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
  "appVersion": "0.19.7338.23496",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```
##### <a name="response"></a><span data-ttu-id="adcdd-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="adcdd-155">Response</span></span>
<span data-ttu-id="adcdd-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="adcdd-156">The following is an example of the response.</span></span>
><span data-ttu-id="adcdd-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="adcdd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printConnector"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 406

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/connectors/$entity",
  "id": "9953d245-3f6e-418c-a438-67f50e69a430",
  "name": "ConnectorName",
  "fullyQualifiedDomainName": "CONNECTOR-MACHINE",
  "operatingSystem": "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555",
  "appVersion": "0.19.7338.23496",
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
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
  },
  "registeredBy": {}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update printConnector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->