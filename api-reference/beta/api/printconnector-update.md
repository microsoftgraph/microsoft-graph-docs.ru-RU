---
title: Обновление printConnector
description: Обновление свойств объекта printConnector.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 767f60c6db7b212cd33467bdad893fc8c8ac853b
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873551"
---
# <a name="update-printconnector"></a><span data-ttu-id="60697-103">Обновление printConnector</span><span class="sxs-lookup"><span data-stu-id="60697-103">Update printConnector</span></span>

<span data-ttu-id="60697-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60697-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60697-105">Обновление свойств объекта **printConnector.**</span><span class="sxs-lookup"><span data-stu-id="60697-105">Update the properties of a **printConnector** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="60697-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60697-106">Permissions</span></span>
<span data-ttu-id="60697-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60697-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="60697-109">Чтобы использовать службу универсальной печати, у пользователя или клиента приложения должна быть активная подписка универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="60697-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="60697-110">Пользователь, выписав его, должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="60697-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="60697-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60697-111">Permission type</span></span> | <span data-ttu-id="60697-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60697-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="60697-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60697-113">Delegated (work or school account)</span></span>| <span data-ttu-id="60697-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60697-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="60697-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60697-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60697-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60697-116">Not Supported.</span></span>|
|<span data-ttu-id="60697-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="60697-117">Application</span></span>|<span data-ttu-id="60697-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60697-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60697-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60697-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/connectors/{id}
```
## <a name="request-headers"></a><span data-ttu-id="60697-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60697-120">Request headers</span></span>
| <span data-ttu-id="60697-121">Имя</span><span class="sxs-lookup"><span data-stu-id="60697-121">Name</span></span>       | <span data-ttu-id="60697-122">Описание</span><span class="sxs-lookup"><span data-stu-id="60697-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="60697-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60697-123">Authorization</span></span> | <span data-ttu-id="60697-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60697-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="60697-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="60697-126">Content-type</span></span>  | <span data-ttu-id="60697-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60697-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="60697-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60697-129">Request body</span></span>
<span data-ttu-id="60697-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="60697-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="60697-131">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="60697-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="60697-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="60697-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="60697-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="60697-133">Property</span></span>     | <span data-ttu-id="60697-134">Тип</span><span class="sxs-lookup"><span data-stu-id="60697-134">Type</span></span>        | <span data-ttu-id="60697-135">Описание</span><span class="sxs-lookup"><span data-stu-id="60697-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="60697-136">name</span><span class="sxs-lookup"><span data-stu-id="60697-136">name</span></span>|<span data-ttu-id="60697-137">String</span><span class="sxs-lookup"><span data-stu-id="60697-137">String</span></span>|<span data-ttu-id="60697-138">Имя соединители.</span><span class="sxs-lookup"><span data-stu-id="60697-138">The name of the connector.</span></span>|
|<span data-ttu-id="60697-139">fullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="60697-139">fullyQualifiedDomainName</span></span>|<span data-ttu-id="60697-140">String</span><span class="sxs-lookup"><span data-stu-id="60697-140">String</span></span>|<span data-ttu-id="60697-141">Имя хоста компьютера соединитела.</span><span class="sxs-lookup"><span data-stu-id="60697-141">The connector machine's hostname.</span></span>|
|<span data-ttu-id="60697-142">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="60697-142">operatingSystem</span></span>|<span data-ttu-id="60697-143">String</span><span class="sxs-lookup"><span data-stu-id="60697-143">String</span></span>|<span data-ttu-id="60697-144">Версия операционной системы компьютера соединители.</span><span class="sxs-lookup"><span data-stu-id="60697-144">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="60697-145">appVersion</span><span class="sxs-lookup"><span data-stu-id="60697-145">appVersion</span></span>|<span data-ttu-id="60697-146">String</span><span class="sxs-lookup"><span data-stu-id="60697-146">String</span></span>|<span data-ttu-id="60697-147">Версия соединители.</span><span class="sxs-lookup"><span data-stu-id="60697-147">The connector's version.</span></span>|
|<span data-ttu-id="60697-148">location</span><span class="sxs-lookup"><span data-stu-id="60697-148">location</span></span>|[<span data-ttu-id="60697-149">printerLocation</span><span class="sxs-lookup"><span data-stu-id="60697-149">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="60697-150">Физическое и/или организационное расположение соединители.</span><span class="sxs-lookup"><span data-stu-id="60697-150">The physical and/or organizational location of the connector.</span></span>|

## <a name="response"></a><span data-ttu-id="60697-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="60697-151">Response</span></span>
<span data-ttu-id="60697-152">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект printConnector](../resources/printConnector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="60697-152">If successful, this method returns a `200 OK` response code and an updated [printConnector](../resources/printConnector.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="60697-153">Пример</span><span class="sxs-lookup"><span data-stu-id="60697-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60697-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="60697-154">Request</span></span>
<span data-ttu-id="60697-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60697-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="60697-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="60697-156">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="60697-157">C#</span><span class="sxs-lookup"><span data-stu-id="60697-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60697-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60697-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60697-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60697-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60697-160">Java</span><span class="sxs-lookup"><span data-stu-id="60697-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-connector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="60697-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="60697-161">Response</span></span>
<span data-ttu-id="60697-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="60697-162">The following is an example of the response.</span></span>
><span data-ttu-id="60697-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="60697-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
