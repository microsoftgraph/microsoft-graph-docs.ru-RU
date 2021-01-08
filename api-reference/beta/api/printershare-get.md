---
title: Получение printerShare
description: Извлечение свойств и связей из обоймы принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: a30f670d429fb57d92c7c0cf5f615ffb60bb2d59
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784866"
---
# <a name="get-printershare"></a><span data-ttu-id="de3f6-103">Получение printerShare</span><span class="sxs-lookup"><span data-stu-id="de3f6-103">Get printerShare</span></span>

<span data-ttu-id="de3f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de3f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de3f6-105">Извлечение свойств и связей из обоймы принтера.</span><span class="sxs-lookup"><span data-stu-id="de3f6-105">Retrieve the properties and relationships of a printer share.</span></span>

## <a name="permissions"></a><span data-ttu-id="de3f6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de3f6-106">Permissions</span></span>
<span data-ttu-id="de3f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de3f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="de3f6-109">Помимо следующих разрешений, у пользователя или клиента приложения должна быть активная подписка универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="de3f6-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="de3f6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de3f6-110">Permission type</span></span> | <span data-ttu-id="de3f6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de3f6-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="de3f6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de3f6-112">Delegated (work or school account)</span></span>| <span data-ttu-id="de3f6-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de3f6-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="de3f6-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de3f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de3f6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de3f6-115">Not Supported.</span></span>|
|<span data-ttu-id="de3f6-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="de3f6-116">Application</span></span>|<span data-ttu-id="de3f6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de3f6-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de3f6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de3f6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{id}
GET /print/printers/{id}/share
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de3f6-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="de3f6-119">Optional query parameters</span></span>
<span data-ttu-id="de3f6-120">Этот метод поддерживает некоторые параметры запроса OData, в том числе $select, $expand для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="de3f6-120">This method supports some of the OData query parameters including $select, $expand to help customize the response.</span></span> <span data-ttu-id="de3f6-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="de3f6-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="de3f6-122">например,</span><span class="sxs-lookup"><span data-stu-id="de3f6-122">e.g.</span></span> 
```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```

### <a name="exceptions"></a><span data-ttu-id="de3f6-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="de3f6-123">Exceptions</span></span>
* <span data-ttu-id="de3f6-124">Оператор `$count` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de3f6-124">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de3f6-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de3f6-125">Request headers</span></span>
| <span data-ttu-id="de3f6-126">Имя</span><span class="sxs-lookup"><span data-stu-id="de3f6-126">Name</span></span>      |<span data-ttu-id="de3f6-127">Описание</span><span class="sxs-lookup"><span data-stu-id="de3f6-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="de3f6-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de3f6-128">Authorization</span></span> | <span data-ttu-id="de3f6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de3f6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de3f6-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="de3f6-131">Request body</span></span>
<span data-ttu-id="de3f6-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de3f6-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="de3f6-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="de3f6-133">Response</span></span>
<span data-ttu-id="de3f6-134">В случае успеха этот метод возвращает код отклика и объект `200 OK` [printerShare](../resources/printershare.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de3f6-134">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>
<span data-ttu-id="de3f6-135">По умолчанию отклик не будет содержать [printerCapabilities.](../resources/printerCapabilities.md)</span><span class="sxs-lookup"><span data-stu-id="de3f6-135">By default, the response will not contain [printerCapabilities](../resources/printerCapabilities.md).</span></span> <span data-ttu-id="de3f6-136">Чтобы получить **printerCapabilities,** используйте параметр `$select` запроса.</span><span class="sxs-lookup"><span data-stu-id="de3f6-136">To get **printerCapabilities**, use the `$select` query parameter.</span></span> 

## <a name="example"></a><span data-ttu-id="de3f6-137">Пример</span><span class="sxs-lookup"><span data-stu-id="de3f6-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="de3f6-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="de3f6-138">Request</span></span>
<span data-ttu-id="de3f6-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de3f6-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="de3f6-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="de3f6-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printershare"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}
```
# <a name="c"></a>[<span data-ttu-id="de3f6-141">C#</span><span class="sxs-lookup"><span data-stu-id="de3f6-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de3f6-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de3f6-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de3f6-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de3f6-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="de3f6-144">Java</span><span class="sxs-lookup"><span data-stu-id="de3f6-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="de3f6-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="de3f6-145">Response</span></span>
<span data-ttu-id="de3f6-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="de3f6-146">The following is an example of the response.</span></span>
><span data-ttu-id="de3f6-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de3f6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z"
}
```

<span data-ttu-id="de3f6-149">Ниже приводится пример ответа при использовании $select=id,displayName,capabilities</span><span class="sxs-lookup"><span data-stu-id="de3f6-149">The following is an example of the response, when using $select=id,displayName,capabilities</span></span>
><span data-ttu-id="de3f6-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de3f6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "ShareName",
  "capabilities": {
    "isColorPrintingSupported": true,
    "supportsFitPdfToPage": false,
    "contentTypes": [
      "application/pdf",
      "image/pwg-raster",
      "application/PCLm"
    ],
    "isPageRangeSupported": false,
    "qualities": [
      "medium"
    ],
    "dpis": [
      600
    ],
    "duplexModes": [
      "oneSided",
      "flipOnLongEdge",
      "flipOnShortEdge"
    ],
    "finishings": [
      "none"
    ],
    "mediaTypes": [
      "stationery"
    ],
    "mediaSizes": [
      "North America Letter"
    ],
    "outputBins": [
      "tray-1"
    ],
    "colorModes": [
      "grayscale",
      "color"
    ],
    "inputBins": [
      "tray-1"
    ],
    "collation": true,
    "scalings": [
      "fill"
    ],
    "copiesPerJob": {
      "start": 1,
      "end": 38
    }
  }
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


