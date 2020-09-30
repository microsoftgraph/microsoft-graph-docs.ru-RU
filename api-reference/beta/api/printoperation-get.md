---
title: Получение Принтоператион
description: Получение объекта Принтоператион.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 4622c428c91ef1290dc4a824f3a37b07403d2ea1
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314547"
---
# <a name="get-printoperation"></a><span data-ttu-id="95d42-103">Получение Принтоператион</span><span class="sxs-lookup"><span data-stu-id="95d42-103">Get printOperation</span></span>

<span data-ttu-id="95d42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95d42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95d42-105">Получение свойств и связей объекта [принтоператион](../resources/printoperation.md) .</span><span class="sxs-lookup"><span data-stu-id="95d42-105">Retrieve the properties and relationships of a [printOperation](../resources/printoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="95d42-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95d42-106">Permissions</span></span>
<span data-ttu-id="95d42-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95d42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="95d42-109">Пользователь, вошедшего в систему, должен быть [администратором принтера](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="95d42-109">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="95d42-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95d42-110">Permission type</span></span> | <span data-ttu-id="95d42-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95d42-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="95d42-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95d42-112">Delegated (work or school account)</span></span>| <span data-ttu-id="95d42-113">Printer. Create, Printer. ReadWrite. ALL, Printer. FullControl. ALL</span><span class="sxs-lookup"><span data-stu-id="95d42-113">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="95d42-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95d42-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95d42-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95d42-115">Not Supported.</span></span>|
|<span data-ttu-id="95d42-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95d42-116">Application</span></span>| <span data-ttu-id="95d42-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95d42-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="95d42-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95d42-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/operations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="95d42-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95d42-119">Request headers</span></span>
| <span data-ttu-id="95d42-120">Имя</span><span class="sxs-lookup"><span data-stu-id="95d42-120">Name</span></span>      |<span data-ttu-id="95d42-121">Описание</span><span class="sxs-lookup"><span data-stu-id="95d42-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="95d42-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95d42-122">Authorization</span></span> | <span data-ttu-id="95d42-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95d42-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="95d42-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95d42-125">Request body</span></span>
<span data-ttu-id="95d42-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="95d42-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="95d42-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="95d42-127">Response</span></span>
<span data-ttu-id="95d42-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [принтоператион](../resources/printOperation.md) (или производный от **принтоператион**) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="95d42-128">If successful, this method returns a `200 OK` response code and a [printOperation](../resources/printOperation.md) object (or a derivative of **printOperation**) in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="95d42-129">Пример</span><span class="sxs-lookup"><span data-stu-id="95d42-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="95d42-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="95d42-130">Request</span></span>
<span data-ttu-id="95d42-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95d42-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="95d42-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="95d42-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/operations/{id}
```
# <a name="c"></a>[<span data-ttu-id="95d42-133">C#</span><span class="sxs-lookup"><span data-stu-id="95d42-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95d42-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95d42-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95d42-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95d42-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="95d42-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="95d42-136">Response</span></span>
<span data-ttu-id="95d42-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="95d42-137">The following is an example of the response.</span></span>
><span data-ttu-id="95d42-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95d42-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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