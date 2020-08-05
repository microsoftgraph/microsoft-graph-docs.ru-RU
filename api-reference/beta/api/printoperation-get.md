---
title: Получение Принтоператион
description: Получение объекта Принтоператион.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: dd03367e71a9c5273e294ac022d4ac9d8a5e2760
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565646"
---
# <a name="get-printoperation"></a><span data-ttu-id="bcced-103">Получение Принтоператион</span><span class="sxs-lookup"><span data-stu-id="bcced-103">Get printOperation</span></span>

<span data-ttu-id="bcced-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcced-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcced-105">Получение свойств и связей объекта [принтоператион](../resources/printoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="bcced-105">Retrieve the properties and relationships of a [printOperation](../resources/printoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcced-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bcced-106">Permissions</span></span>
<span data-ttu-id="bcced-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcced-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcced-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcced-109">Permission type</span></span> | <span data-ttu-id="bcced-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcced-110">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="bcced-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcced-111">Delegated (work or school account)</span></span>| <span data-ttu-id="bcced-112">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcced-112">User.Read.All</span></span> |
|<span data-ttu-id="bcced-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcced-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcced-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcced-114">Not Supported.</span></span>|
|<span data-ttu-id="bcced-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcced-115">Application</span></span>|<span data-ttu-id="bcced-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcced-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcced-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcced-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/operations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bcced-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcced-118">Request headers</span></span>
| <span data-ttu-id="bcced-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bcced-119">Name</span></span>      |<span data-ttu-id="bcced-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bcced-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bcced-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bcced-121">Authorization</span></span> | <span data-ttu-id="bcced-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcced-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bcced-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bcced-124">Request body</span></span>
<span data-ttu-id="bcced-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bcced-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bcced-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcced-126">Response</span></span>
<span data-ttu-id="bcced-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтоператион](../resources/printOperation.md) (или производный от **принтоператион**) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bcced-127">If successful, this method returns a `200 OK` response code and a [printOperation](../resources/printOperation.md) object (or a derivative of **printOperation**) in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bcced-128">Пример</span><span class="sxs-lookup"><span data-stu-id="bcced-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="bcced-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcced-129">Request</span></span>
<span data-ttu-id="bcced-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcced-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bcced-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcced-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/operations/{id}
```
# <a name="c"></a>[<span data-ttu-id="bcced-132">C#</span><span class="sxs-lookup"><span data-stu-id="bcced-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bcced-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcced-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bcced-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcced-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bcced-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcced-135">Response</span></span>
<span data-ttu-id="bcced-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bcced-136">The following is an example of the response.</span></span>
><span data-ttu-id="bcced-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bcced-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1199

{
    "@odata.context": "https://graph.microsoft-ppe.com/beta/$metadata#print/operations/$entity",
    "@odata.type": "#microsoft.graph.printerCreateOperation",
    "id": "81f4cca3-b3b7-47ea-9f88-7ddbf7208ef4",
    "createdDateTime": "2020-06-15T22:27:03.031849Z",
    "certificate": "{ceritificate}",
    "status": {
        "state": "succeeded",
        "description": "The operation has completed successfully."
    },
    "printer": {
        "registeredDateTime": "2020-06-15T22:27:12.0920077Z",
        "acceptingJobs": null,
        "isShared": false,
        "id": "e56f9cdd-acec-486f-a05e-b622ff0bcc7d",
        "name": "Test Printer",
        "manufacturer": "Test Printer Manufacturer",
        "model": "Test Printer Model",
        "isAcceptingJobs": null,
        "capabilities": null,
        "status": {
            "processingState": "unknown",
            "processingStateReasons": [],
            "processingStateDescription": ""
        },
        "location": {
            "latitude": null,
            "longitude": null
        },
        "defaults": {
            "copiesPerJob": 1,
            "finishings": []
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
