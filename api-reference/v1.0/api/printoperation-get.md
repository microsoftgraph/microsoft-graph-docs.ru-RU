---
title: Get printOperation
description: Извлечение printOperation.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: ccd4960f4b8da00b2352feda7bb6106523958dcc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771367"
---
# <a name="get-printoperation"></a><span data-ttu-id="9a93b-103">Get printOperation</span><span class="sxs-lookup"><span data-stu-id="9a93b-103">Get printOperation</span></span>
<span data-ttu-id="9a93b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a93b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="9a93b-105">Извлечение свойств и связей объекта [printOperation.](../resources/printoperation.md)</span><span class="sxs-lookup"><span data-stu-id="9a93b-105">Retrieve the properties and relationships of a [printOperation](../resources/printoperation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a93b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a93b-106">Permissions</span></span>
<span data-ttu-id="9a93b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a93b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="9a93b-109">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="9a93b-109">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="9a93b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a93b-110">Permission type</span></span> | <span data-ttu-id="9a93b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a93b-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="9a93b-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a93b-112">Delegated (work or school account)</span></span>| <span data-ttu-id="9a93b-113">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="9a93b-113">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="9a93b-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a93b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a93b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a93b-115">Not Supported.</span></span>|
|<span data-ttu-id="9a93b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a93b-116">Application</span></span>| <span data-ttu-id="9a93b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a93b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a93b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a93b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/operations/{printOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="9a93b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a93b-119">Request headers</span></span>
|<span data-ttu-id="9a93b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9a93b-120">Name</span></span>|<span data-ttu-id="9a93b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9a93b-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9a93b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a93b-122">Authorization</span></span>|<span data-ttu-id="9a93b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a93b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a93b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a93b-125">Request body</span></span>
<span data-ttu-id="9a93b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a93b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a93b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a93b-127">Response</span></span>
<span data-ttu-id="9a93b-128">В случае успеха этот метод возвращает код отклика и объект `200 OK` [printOperation](../resources/printOperation.md) (или производный **printOperation)** в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9a93b-128">If successful, this method returns a `200 OK` response code and a [printOperation](../resources/printOperation.md) object (or a derivative of **printOperation**) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a93b-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="9a93b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9a93b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a93b-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9a93b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a93b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printoperation"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/operations/{printOperationId}
```
# <a name="c"></a>[<span data-ttu-id="9a93b-132">C#</span><span class="sxs-lookup"><span data-stu-id="9a93b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a93b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a93b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a93b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a93b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a93b-135">Java</span><span class="sxs-lookup"><span data-stu-id="9a93b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9a93b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a93b-136">Response</span></span>
<span data-ttu-id="9a93b-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9a93b-137">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printOperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/operations/$entity",
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

