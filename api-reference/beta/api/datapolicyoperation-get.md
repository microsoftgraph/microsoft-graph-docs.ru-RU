---
title: Получение dataPolicyOperation
description: Получение свойств объекта dataPolicyOperation.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 08cfbf935a1a37be83349d2d75631bc8767ec8d8
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123687"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="6af1d-103">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="6af1d-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="6af1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6af1d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6af1d-105">Получение свойств объекта dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="6af1d-105">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6af1d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6af1d-106">Permissions</span></span>
<span data-ttu-id="6af1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6af1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6af1d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6af1d-109">Permission type</span></span>      | <span data-ttu-id="6af1d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6af1d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6af1d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6af1d-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="6af1d-112">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="6af1d-112">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="6af1d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6af1d-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6af1d-114">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="6af1d-114">Not applicable</span></span>  |
|<span data-ttu-id="6af1d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6af1d-115">Application</span></span> | <span data-ttu-id="6af1d-116">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="6af1d-116">User.Export.All and User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6af1d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6af1d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6af1d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6af1d-118">Request headers</span></span>
| <span data-ttu-id="6af1d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6af1d-119">Name</span></span>      |<span data-ttu-id="6af1d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6af1d-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6af1d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6af1d-121">Authorization</span></span>  | <span data-ttu-id="6af1d-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6af1d-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6af1d-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6af1d-123">Request body</span></span>
<span data-ttu-id="6af1d-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6af1d-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6af1d-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="6af1d-125">Response</span></span>
<span data-ttu-id="6af1d-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [dataPolicyOperation](../resources/datapolicyoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6af1d-126">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6af1d-127">Пример</span><span class="sxs-lookup"><span data-stu-id="6af1d-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6af1d-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="6af1d-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6af1d-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="6af1d-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
# <a name="c"></a>[<span data-ttu-id="6af1d-130">C#</span><span class="sxs-lookup"><span data-stu-id="6af1d-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-datapolicyoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6af1d-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6af1d-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-datapolicyoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6af1d-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6af1d-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-datapolicyoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6af1d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6af1d-133">Response</span></span>
<span data-ttu-id="6af1d-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6af1d-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dataPolicyOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 212

{
  "completedDateTime": "datetime-value",
  "id": "id-value",
  "status": "status-value",
  "storageLocation": "storageLocation-value",
  "userId": "userId-value",
  "submittedDateTime": "datetime-value",
  "progress": "double"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get dataPolicyOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
