---
title: Get printOperation
description: Извлечение printOperation.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 35bc4e58616c79e060548108d81d59f345e20f32
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055304"
---
# <a name="get-printoperation"></a><span data-ttu-id="2df47-103">Get printOperation</span><span class="sxs-lookup"><span data-stu-id="2df47-103">Get printOperation</span></span>

<span data-ttu-id="2df47-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2df47-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2df47-105">Извлечение свойств и связей объекта [printOperation.](../resources/printoperation.md)</span><span class="sxs-lookup"><span data-stu-id="2df47-105">Retrieve the properties and relationships of a [printOperation](../resources/printoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2df47-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2df47-106">Permissions</span></span>
<span data-ttu-id="2df47-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2df47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2df47-109">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="2df47-109">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="2df47-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2df47-110">Permission type</span></span> | <span data-ttu-id="2df47-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2df47-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2df47-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2df47-112">Delegated (work or school account)</span></span>| <span data-ttu-id="2df47-113">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="2df47-113">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="2df47-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2df47-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2df47-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2df47-115">Not Supported.</span></span>|
|<span data-ttu-id="2df47-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2df47-116">Application</span></span>| <span data-ttu-id="2df47-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2df47-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2df47-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2df47-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/operations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2df47-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2df47-119">Request headers</span></span>
| <span data-ttu-id="2df47-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2df47-120">Name</span></span>      |<span data-ttu-id="2df47-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2df47-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2df47-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2df47-122">Authorization</span></span> | <span data-ttu-id="2df47-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2df47-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2df47-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2df47-125">Request body</span></span>
<span data-ttu-id="2df47-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2df47-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2df47-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2df47-127">Response</span></span>
<span data-ttu-id="2df47-128">В случае успеха этот метод возвращает код отклика и объект `200 OK` [printOperation](../resources/printOperation.md) (или производный **printOperation)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2df47-128">If successful, this method returns a `200 OK` response code and a [printOperation](../resources/printOperation.md) object (or a derivative of **printOperation**) in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2df47-129">Пример</span><span class="sxs-lookup"><span data-stu-id="2df47-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="2df47-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="2df47-130">Request</span></span>
<span data-ttu-id="2df47-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2df47-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2df47-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2df47-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/operations/{id}
```
# <a name="c"></a>[<span data-ttu-id="2df47-133">C#</span><span class="sxs-lookup"><span data-stu-id="2df47-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2df47-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2df47-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2df47-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2df47-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2df47-136">Java</span><span class="sxs-lookup"><span data-stu-id="2df47-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2df47-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2df47-137">Response</span></span>
<span data-ttu-id="2df47-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2df47-138">The following is an example of the response.</span></span>
><span data-ttu-id="2df47-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2df47-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/operations/$entity",
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
        "isShared": false,
        "id": "e56f9cdd-acec-486f-a05e-b622ff0bcc7d",
        "displayName": "Test Printer",
        "manufacturer": "Test Printer Manufacturer",
        "model": "Test Printer Model",
        "isAcceptingJobs": null,
        "status": {
            "state": "unknown",
            "details": [],
            "description": ""
        },
        "location": {
            "latitude": null,
            "longitude": null
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
