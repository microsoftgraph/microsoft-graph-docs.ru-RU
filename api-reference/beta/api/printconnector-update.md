---
title: Обновление printConnector
description: Обновление свойств объекта printConnector.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: ad196f179a81f9d5467ba715a08730b09ad4b88c
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766044"
---
# <a name="update-printconnector"></a><span data-ttu-id="5af54-103">Обновление printConnector</span><span class="sxs-lookup"><span data-stu-id="5af54-103">Update printConnector</span></span>

<span data-ttu-id="5af54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5af54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5af54-105">Обновление свойств объекта **printConnector.**</span><span class="sxs-lookup"><span data-stu-id="5af54-105">Update the properties of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5af54-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5af54-106">Permissions</span></span>
<span data-ttu-id="5af54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5af54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5af54-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="5af54-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="5af54-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="5af54-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="5af54-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5af54-111">Permission type</span></span> | <span data-ttu-id="5af54-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5af54-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="5af54-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5af54-113">Delegated (work or school account)</span></span>| <span data-ttu-id="5af54-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5af54-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="5af54-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5af54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5af54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5af54-116">Not Supported.</span></span>|
|<span data-ttu-id="5af54-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5af54-117">Application</span></span>|<span data-ttu-id="5af54-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5af54-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5af54-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5af54-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5af54-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5af54-120">Request headers</span></span>
| <span data-ttu-id="5af54-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5af54-121">Name</span></span>       | <span data-ttu-id="5af54-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5af54-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5af54-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5af54-123">Authorization</span></span> | <span data-ttu-id="5af54-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5af54-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5af54-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5af54-126">Content-type</span></span>  | <span data-ttu-id="5af54-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5af54-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5af54-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5af54-129">Request body</span></span>
<span data-ttu-id="5af54-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="5af54-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5af54-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="5af54-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5af54-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5af54-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5af54-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="5af54-133">Property</span></span>     | <span data-ttu-id="5af54-134">Тип</span><span class="sxs-lookup"><span data-stu-id="5af54-134">Type</span></span>        | <span data-ttu-id="5af54-135">Описание</span><span class="sxs-lookup"><span data-stu-id="5af54-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5af54-136">name</span><span class="sxs-lookup"><span data-stu-id="5af54-136">name</span></span>|<span data-ttu-id="5af54-137">String</span><span class="sxs-lookup"><span data-stu-id="5af54-137">String</span></span>|<span data-ttu-id="5af54-138">Имя соединитетеля.</span><span class="sxs-lookup"><span data-stu-id="5af54-138">The name of the connector.</span></span>|
|<span data-ttu-id="5af54-139">fullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="5af54-139">fullyQualifiedDomainName</span></span>|<span data-ttu-id="5af54-140">String</span><span class="sxs-lookup"><span data-stu-id="5af54-140">String</span></span>|<span data-ttu-id="5af54-141">Имя хост-имени соединители.</span><span class="sxs-lookup"><span data-stu-id="5af54-141">The connector machine's hostname.</span></span>|
|<span data-ttu-id="5af54-142">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="5af54-142">operatingSystem</span></span>|<span data-ttu-id="5af54-143">String</span><span class="sxs-lookup"><span data-stu-id="5af54-143">String</span></span>|<span data-ttu-id="5af54-144">Версия операционной системы соединитетеля.</span><span class="sxs-lookup"><span data-stu-id="5af54-144">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="5af54-145">appVersion</span><span class="sxs-lookup"><span data-stu-id="5af54-145">appVersion</span></span>|<span data-ttu-id="5af54-146">String</span><span class="sxs-lookup"><span data-stu-id="5af54-146">String</span></span>|<span data-ttu-id="5af54-147">Версия соединиттеля.</span><span class="sxs-lookup"><span data-stu-id="5af54-147">The connector's version.</span></span>|
|<span data-ttu-id="5af54-148">расположение</span><span class="sxs-lookup"><span data-stu-id="5af54-148">location</span></span>|[<span data-ttu-id="5af54-149">printerLocation</span><span class="sxs-lookup"><span data-stu-id="5af54-149">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="5af54-150">Физическое и/или организационное расположение соединитетеля.</span><span class="sxs-lookup"><span data-stu-id="5af54-150">The physical and/or organizational location of the connector.</span></span>|

## <a name="response"></a><span data-ttu-id="5af54-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="5af54-151">Response</span></span>
<span data-ttu-id="5af54-152">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [printConnector](../resources/printConnector.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5af54-152">If successful, this method returns a `200 OK` response code and an updated [printConnector](../resources/printConnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5af54-153">Пример</span><span class="sxs-lookup"><span data-stu-id="5af54-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5af54-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="5af54-154">Request</span></span>
<span data-ttu-id="5af54-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5af54-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5af54-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="5af54-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_connector"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/connectors/{id}
Content-type: application/json
Content-length: 300

{
  "displayName": "ConnectorName",
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

---

##### <a name="response"></a><span data-ttu-id="5af54-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="5af54-157">Response</span></span>
<span data-ttu-id="5af54-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5af54-158">The following is an example of the response.</span></span>
><span data-ttu-id="5af54-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5af54-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "displayName": "ConnectorName",
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
    "floor": "1",
    "floorDescription": "First Floor",
    "roomName": "1234",
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
  "description": "Update printConnector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
