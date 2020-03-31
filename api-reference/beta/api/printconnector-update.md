---
title: Обновление Принтконнектор
description: Обновление свойств объекта Принтконнектор.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7b4a9a0b74969877ca1336facda8e63462919b6b
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062128"
---
# <a name="update-printconnector"></a><span data-ttu-id="79ce4-103">Обновление Принтконнектор</span><span class="sxs-lookup"><span data-stu-id="79ce4-103">Update printConnector</span></span>

<span data-ttu-id="79ce4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79ce4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79ce4-105">Обновление свойств объекта **принтконнектор** .</span><span class="sxs-lookup"><span data-stu-id="79ce4-105">Update the properties of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="79ce4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79ce4-106">Permissions</span></span>
<span data-ttu-id="79ce4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79ce4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="79ce4-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="79ce4-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="79ce4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79ce4-110">Permission type</span></span> | <span data-ttu-id="79ce4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79ce4-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="79ce4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79ce4-112">Delegated (work or school account)</span></span>| <span data-ttu-id="79ce4-113">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="79ce4-113">Users.Read.All</span></span> |
|<span data-ttu-id="79ce4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79ce4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79ce4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79ce4-115">Not Supported.</span></span>|
|<span data-ttu-id="79ce4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="79ce4-116">Application</span></span>|<span data-ttu-id="79ce4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79ce4-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79ce4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79ce4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="79ce4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79ce4-119">Request headers</span></span>
| <span data-ttu-id="79ce4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="79ce4-120">Name</span></span>       | <span data-ttu-id="79ce4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="79ce4-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="79ce4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79ce4-122">Authorization</span></span> | <span data-ttu-id="79ce4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79ce4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="79ce4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79ce4-125">Content-type</span></span>  | <span data-ttu-id="79ce4-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79ce4-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="79ce4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79ce4-128">Request body</span></span>
<span data-ttu-id="79ce4-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="79ce4-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="79ce4-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="79ce4-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="79ce4-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="79ce4-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="79ce4-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="79ce4-132">Property</span></span>     | <span data-ttu-id="79ce4-133">Тип</span><span class="sxs-lookup"><span data-stu-id="79ce4-133">Type</span></span>        | <span data-ttu-id="79ce4-134">Описание</span><span class="sxs-lookup"><span data-stu-id="79ce4-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="79ce4-135">name</span><span class="sxs-lookup"><span data-stu-id="79ce4-135">name</span></span>|<span data-ttu-id="79ce4-136">String</span><span class="sxs-lookup"><span data-stu-id="79ce4-136">String</span></span>|<span data-ttu-id="79ce4-137">Имя соединителя.</span><span class="sxs-lookup"><span data-stu-id="79ce4-137">The name of the connector.</span></span>|
|<span data-ttu-id="79ce4-138">fullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="79ce4-138">fullyQualifiedDomainName</span></span>|<span data-ttu-id="79ce4-139">String</span><span class="sxs-lookup"><span data-stu-id="79ce4-139">String</span></span>|<span data-ttu-id="79ce4-140">Имя узла для соединителя.</span><span class="sxs-lookup"><span data-stu-id="79ce4-140">The connector machine's hostname.</span></span>|
|<span data-ttu-id="79ce4-141">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="79ce4-141">operatingSystem</span></span>|<span data-ttu-id="79ce4-142">String</span><span class="sxs-lookup"><span data-stu-id="79ce4-142">String</span></span>|<span data-ttu-id="79ce4-143">Версия операционной системы на соединителе компьютера.</span><span class="sxs-lookup"><span data-stu-id="79ce4-143">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="79ce4-144">аппверсион</span><span class="sxs-lookup"><span data-stu-id="79ce4-144">appVersion</span></span>|<span data-ttu-id="79ce4-145">String</span><span class="sxs-lookup"><span data-stu-id="79ce4-145">String</span></span>|<span data-ttu-id="79ce4-146">Версия соединителя.</span><span class="sxs-lookup"><span data-stu-id="79ce4-146">The connector's version.</span></span>|
|<span data-ttu-id="79ce4-147">расположение;</span><span class="sxs-lookup"><span data-stu-id="79ce4-147">location</span></span>|[<span data-ttu-id="79ce4-148">принтерлокатион</span><span class="sxs-lookup"><span data-stu-id="79ce4-148">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="79ce4-149">Физическое и/или организационное расположение соединителя.</span><span class="sxs-lookup"><span data-stu-id="79ce4-149">The physical and/or organizational location of the connector.</span></span>|

## <a name="response"></a><span data-ttu-id="79ce4-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="79ce4-150">Response</span></span>
<span data-ttu-id="79ce4-151">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [принтконнектор](../resources/printConnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79ce4-151">If successful, this method returns a `200 OK` response code and an updated [printConnector](../resources/printConnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="79ce4-152">Пример</span><span class="sxs-lookup"><span data-stu-id="79ce4-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="79ce4-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="79ce4-153">Request</span></span>
<span data-ttu-id="79ce4-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79ce4-154">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="79ce4-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="79ce4-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="79ce4-156">C#</span><span class="sxs-lookup"><span data-stu-id="79ce4-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79ce4-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79ce4-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79ce4-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79ce4-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="79ce4-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="79ce4-159">Response</span></span>
<span data-ttu-id="79ce4-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="79ce4-160">The following is an example of the response.</span></span>
><span data-ttu-id="79ce4-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79ce4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
