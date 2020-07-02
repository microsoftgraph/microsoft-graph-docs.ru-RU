---
title: Обновление принтера
description: Обновление свойств объекта Printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: fd44a74bd1a0a5a8c872f49515edce23c27d6907
ms.sourcegitcommit: 9f1e02ab486a2c3e0a128e5d36f46cebe4961581
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2020
ms.locfileid: "45024441"
---
# <a name="update-printer"></a><span data-ttu-id="b7c61-103">Обновление принтера</span><span class="sxs-lookup"><span data-stu-id="b7c61-103">Update printer</span></span>

<span data-ttu-id="b7c61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7c61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7c61-105">Обновление свойств объекта [Printer](../resources/printer.md) .</span><span class="sxs-lookup"><span data-stu-id="b7c61-105">Update the properties of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7c61-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7c61-106">Permissions</span></span>
<span data-ttu-id="b7c61-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b7c61-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b7c61-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7c61-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b7c61-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="b7c61-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> 

<span data-ttu-id="b7c61-110">Только приложение, которое зарегистрировало принтер, может обновлять принтер с помощью разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="b7c61-110">Only the app that registered the printer is allowed to update the printer using application permissions.</span></span>

|<span data-ttu-id="b7c61-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7c61-111">Permission type</span></span> | <span data-ttu-id="b7c61-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7c61-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b7c61-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7c61-113">Delegated (work or school account)</span></span>| <span data-ttu-id="b7c61-114">Users. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="b7c61-114">Users.Read.All</span></span> |
|<span data-ttu-id="b7c61-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7c61-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7c61-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7c61-116">Not Supported.</span></span>|
|<span data-ttu-id="b7c61-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7c61-117">Application</span></span>|<span data-ttu-id="b7c61-118">Printer. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b7c61-118">Printer.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7c61-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7c61-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b7c61-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7c61-120">Request headers</span></span>
| <span data-ttu-id="b7c61-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b7c61-121">Name</span></span>       | <span data-ttu-id="b7c61-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b7c61-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b7c61-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7c61-123">Authorization</span></span> | <span data-ttu-id="b7c61-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="b7c61-124">Bearer {token}.</span></span> <span data-ttu-id="b7c61-125">Required.</span><span class="sxs-lookup"><span data-stu-id="b7c61-125">Required.</span></span> |
| <span data-ttu-id="b7c61-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b7c61-126">Content-type</span></span>  | <span data-ttu-id="b7c61-127">`application/json`При использовании делегированных разрешений `application/ipp` при использовании разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="b7c61-127">`application/json` when using delegated permissions, `application/ipp` when using application permissions.</span></span> <span data-ttu-id="b7c61-128">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="b7c61-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7c61-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7c61-129">Request body</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="b7c61-130">Делегированные разрешения и полезные данные JSON</span><span class="sxs-lookup"><span data-stu-id="b7c61-130">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="b7c61-131">Если в тексте запроса используется делегированные разрешения, укажите значения для соответствующих полей [принтера](../resources/printer.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="b7c61-131">If using delegated permissions, in the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="b7c61-132">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="b7c61-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b7c61-133">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="b7c61-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b7c61-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7c61-134">Property</span></span>     | <span data-ttu-id="b7c61-135">Тип</span><span class="sxs-lookup"><span data-stu-id="b7c61-135">Type</span></span>        | <span data-ttu-id="b7c61-136">Описание</span><span class="sxs-lookup"><span data-stu-id="b7c61-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b7c61-137">location</span><span class="sxs-lookup"><span data-stu-id="b7c61-137">location</span></span>|[<span data-ttu-id="b7c61-138">принтерлокатион</span><span class="sxs-lookup"><span data-stu-id="b7c61-138">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="b7c61-139">Физическое и/или организационное расположение принтера.</span><span class="sxs-lookup"><span data-stu-id="b7c61-139">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="b7c61-140">name</span><span class="sxs-lookup"><span data-stu-id="b7c61-140">name</span></span>|<span data-ttu-id="b7c61-141">String</span><span class="sxs-lookup"><span data-stu-id="b7c61-141">String</span></span>|<span data-ttu-id="b7c61-142">Имя принтера.</span><span class="sxs-lookup"><span data-stu-id="b7c61-142">The name of the printer.</span></span>|

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="b7c61-143">Разрешения приложений и полезные данные IPP</span><span class="sxs-lookup"><span data-stu-id="b7c61-143">Application permissions and IPP payload</span></span>

<span data-ttu-id="b7c61-144">При использовании разрешений приложения текст запроса содержит двоичный поток, представляющий группу атрибутов принтера в [кодировке IPP](https://tools.ietf.org/html/rfc8010).</span><span class="sxs-lookup"><span data-stu-id="b7c61-144">If using application permissions, the request body contains a binary stream representing the Printer Attributes group in [IPP encoding](https://tools.ietf.org/html/rfc8010).</span></span>

<span data-ttu-id="b7c61-145">Клиент должен предоставить набор атрибутов принтера с одним или несколькими значениями (включая явно разрешенные значения из диапазона), как определено в [разделе RFC8011 section 4,2](https://tools.ietf.org/html/rfc8011#section-4.2) атрибуты шаблона задания ("XXX-Default", "XXX-supported" и "XXX-Ready"), [section 4,4](https://tools.ietf.org/html/rfc8011#section-4.4) атрибуты описания принтера и все расширения атрибутов, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="b7c61-145">The client MUST supply a set of Printer attributes with one or more values (including explicitly allowed out-of-band values) as defined in [RFC8011 section 4.2](https://tools.ietf.org/html/rfc8011#section-4.2) Job Template Attributes ("xxx-default", "xxx-supported", and "xxx-ready" attributes), [Section 4.4](https://tools.ietf.org/html/rfc8011#section-4.4) Printer Description Attributes, and any attribute extensions supported by the Printer.</span></span> <span data-ttu-id="b7c61-146">Значения каждого из указанных атрибутов принтера заменяют значения соответствующего атрибута принтера для целевого объекта Printer.</span><span class="sxs-lookup"><span data-stu-id="b7c61-146">The value(s) of each Printer attribute supplied replaces the value(s) of the corresponding Printer attribute on the target Printer object.</span></span> <span data-ttu-id="b7c61-147">Для атрибутов, которые могут иметь несколько значений (1setOf), все значения, предоставляемые клиентом, заменяют все значения атрибута соответствующего объекта Printer.</span><span class="sxs-lookup"><span data-stu-id="b7c61-147">For attributes that can have multiple values (1setOf), all values supplied by the client replace all values of the corresponding Printer object attribute.</span></span>

## <a name="response"></a><span data-ttu-id="b7c61-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7c61-148">Response</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="b7c61-149">Делегированные разрешения и полезные данные JSON</span><span class="sxs-lookup"><span data-stu-id="b7c61-149">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="b7c61-150">При успешном использовании делегированных разрешений этот метод возвращает `200 OK` код отклика и обновленный объект [Printer](../resources/printer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b7c61-150">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="b7c61-151">Разрешения приложений и полезные данные IPP</span><span class="sxs-lookup"><span data-stu-id="b7c61-151">Application permissions and IPP payload</span></span>

<span data-ttu-id="b7c61-152">Если при успешном использовании разрешений приложения этот метод возвращает `204 No content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="b7c61-152">If using application permissions, if successful, this method returns `204 No content` response code.</span></span> <span data-ttu-id="b7c61-153">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b7c61-153">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7c61-154">Пример</span><span class="sxs-lookup"><span data-stu-id="b7c61-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7c61-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7c61-155">Request</span></span>
<span data-ttu-id="b7c61-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7c61-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b7c61-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7c61-157">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b7c61-158">C#</span><span class="sxs-lookup"><span data-stu-id="b7c61-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b7c61-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7c61-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b7c61-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7c61-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b7c61-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7c61-161">Response</span></span>
<span data-ttu-id="b7c61-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b7c61-162">The following is an example of the response.</span></span>
><span data-ttu-id="b7c61-163">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="b7c61-163">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b7c61-164">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b7c61-164">All the properties will be returned from an actual call.</span></span>
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
