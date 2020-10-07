---
title: Обновление принтера
description: Обновление свойств объекта Printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: e908ce1b6364041a94a8d6ab42c8da04853b8b6a
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372833"
---
# <a name="update-printer"></a><span data-ttu-id="fbb3e-103">Обновление принтера</span><span class="sxs-lookup"><span data-stu-id="fbb3e-103">Update printer</span></span>

<span data-ttu-id="fbb3e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbb3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbb3e-105">Обновление свойств объекта [Printer](../resources/printer.md) .</span><span class="sxs-lookup"><span data-stu-id="fbb3e-105">Update the properties of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbb3e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fbb3e-106">Permissions</span></span>
<span data-ttu-id="fbb3e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbb3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="fbb3e-109">В дополнение к следующим разрешениям клиент пользователя должен иметь активную универсальную подписку на печать.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="fbb3e-110">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="fbb3e-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="fbb3e-111">Только приложение, которое зарегистрировало принтер, может обновлять принтер с помощью разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-111">Only the app that registered the printer is allowed to update the printer using application permissions.</span></span>

|<span data-ttu-id="fbb3e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbb3e-112">Permission type</span></span> | <span data-ttu-id="fbb3e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbb3e-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="fbb3e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbb3e-114">Delegated (work or school account)</span></span>| <span data-ttu-id="fbb3e-115">Printer. ReadWrite. ALL, Printer. FullControl. ALL</span><span class="sxs-lookup"><span data-stu-id="fbb3e-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="fbb3e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbb3e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbb3e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-117">Not Supported.</span></span>|
|<span data-ttu-id="fbb3e-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="fbb3e-118">Application</span></span>| <span data-ttu-id="fbb3e-119">Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbb3e-119">Printer.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbb3e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbb3e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fbb3e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbb3e-121">Request headers</span></span>
| <span data-ttu-id="fbb3e-122">Имя</span><span class="sxs-lookup"><span data-stu-id="fbb3e-122">Name</span></span>       | <span data-ttu-id="fbb3e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fbb3e-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fbb3e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbb3e-124">Authorization</span></span> | <span data-ttu-id="fbb3e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fbb3e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fbb3e-127">Content-type</span></span>  | <span data-ttu-id="fbb3e-128">`application/json` При использовании делегированных разрешений `application/ipp` при использовании разрешений приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-128">`application/json` when using delegated permissions, `application/ipp` when using application permissions.</span></span> <span data-ttu-id="fbb3e-129">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbb3e-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fbb3e-130">Request body</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="fbb3e-131">Делегированные разрешения и полезные данные JSON</span><span class="sxs-lookup"><span data-stu-id="fbb3e-131">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="fbb3e-132">Если в тексте запроса используется делегированные разрешения, укажите значения для соответствующих полей [принтера](../resources/printer.md) , которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-132">If using delegated permissions, in the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="fbb3e-133">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="fbb3e-134">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fbb3e-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbb3e-135">Property</span></span>     | <span data-ttu-id="fbb3e-136">Тип</span><span class="sxs-lookup"><span data-stu-id="fbb3e-136">Type</span></span>        | <span data-ttu-id="fbb3e-137">Описание</span><span class="sxs-lookup"><span data-stu-id="fbb3e-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fbb3e-138">location</span><span class="sxs-lookup"><span data-stu-id="fbb3e-138">location</span></span>|[<span data-ttu-id="fbb3e-139">принтерлокатион</span><span class="sxs-lookup"><span data-stu-id="fbb3e-139">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="fbb3e-140">Физическое и/или организационное расположение принтера.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-140">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="fbb3e-141">name</span><span class="sxs-lookup"><span data-stu-id="fbb3e-141">name</span></span>|<span data-ttu-id="fbb3e-142">String</span><span class="sxs-lookup"><span data-stu-id="fbb3e-142">String</span></span>|<span data-ttu-id="fbb3e-143">Имя принтера.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-143">The name of the printer.</span></span>|

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="fbb3e-144">Разрешения приложений и полезные данные IPP</span><span class="sxs-lookup"><span data-stu-id="fbb3e-144">Application permissions and IPP payload</span></span>

<span data-ttu-id="fbb3e-145">При использовании разрешений приложения текст запроса содержит двоичный поток, представляющий группу атрибутов принтера в [кодировке IPP](https://tools.ietf.org/html/rfc8010).</span><span class="sxs-lookup"><span data-stu-id="fbb3e-145">If using application permissions, the request body contains a binary stream representing the Printer Attributes group in [IPP encoding](https://tools.ietf.org/html/rfc8010).</span></span>

<span data-ttu-id="fbb3e-146">Клиент должен предоставить набор атрибутов принтера с одним или несколькими значениями (включая явно разрешенные значения из диапазона), как определено в [разделе RFC8011 section 5,2](https://tools.ietf.org/html/rfc8011#section-5.2) атрибуты шаблона задания ("XXX-Default", "XXX-supported" и "XXX-Ready"), [Section 5,4](https://tools.ietf.org/html/rfc8011#section-5.4) атрибуты описания принтера и все расширения атрибутов, поддерживаемые принтером.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-146">The client MUST supply a set of Printer attributes with one or more values (including explicitly allowed out-of-band values) as defined in [RFC8011 section 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) Job Template Attributes ("xxx-default", "xxx-supported", and "xxx-ready" attributes), [Section 5.4](https://tools.ietf.org/html/rfc8011#section-5.4) Printer Description Attributes, and any attribute extensions supported by the Printer.</span></span> <span data-ttu-id="fbb3e-147">Значения каждого из указанных атрибутов принтера заменяют значения соответствующего атрибута принтера для целевого объекта Printer.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-147">The value(s) of each Printer attribute supplied replaces the value(s) of the corresponding Printer attribute on the target Printer object.</span></span> <span data-ttu-id="fbb3e-148">Для атрибутов, которые могут иметь несколько значений (1setOf), все значения, предоставляемые клиентом, заменяют все значения атрибута соответствующего объекта Printer.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-148">For attributes that can have multiple values (1setOf), all values supplied by the client replace all values of the corresponding Printer object attribute.</span></span>

## <a name="response"></a><span data-ttu-id="fbb3e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbb3e-149">Response</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="fbb3e-150">Делегированные разрешения и полезные данные JSON</span><span class="sxs-lookup"><span data-stu-id="fbb3e-150">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="fbb3e-151">При успешном использовании делегированных разрешений этот метод возвращает `200 OK` код отклика и обновленный объект [Printer](../resources/printer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-151">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="fbb3e-152">Разрешения приложений и полезные данные IPP</span><span class="sxs-lookup"><span data-stu-id="fbb3e-152">Application permissions and IPP payload</span></span>

<span data-ttu-id="fbb3e-153">Если при успешном использовании разрешений приложения этот метод возвращает `204 No content` код отклика.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-153">If using application permissions, if successful, this method returns `204 No content` response code.</span></span> <span data-ttu-id="fbb3e-154">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-154">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbb3e-155">Пример</span><span class="sxs-lookup"><span data-stu-id="fbb3e-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbb3e-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbb3e-156">Request</span></span>
<span data-ttu-id="fbb3e-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fbb3e-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="fbb3e-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fbb3e-159">C#</span><span class="sxs-lookup"><span data-stu-id="fbb3e-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fbb3e-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbb3e-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fbb3e-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fbb3e-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="fbb3e-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbb3e-162">Response</span></span>
<span data-ttu-id="fbb3e-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-163">The following is an example of the response.</span></span>
><span data-ttu-id="fbb3e-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbb3e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
