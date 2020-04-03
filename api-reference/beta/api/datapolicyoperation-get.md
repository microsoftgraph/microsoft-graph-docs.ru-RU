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
# <a name="get-datapolicyoperation"></a><span data-ttu-id="a151c-103">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="a151c-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="a151c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a151c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a151c-105">Получение свойств объекта dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="a151c-105">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a151c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a151c-106">Permissions</span></span>
<span data-ttu-id="a151c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a151c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a151c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a151c-109">Permission type</span></span>      | <span data-ttu-id="a151c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a151c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a151c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a151c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="a151c-112">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="a151c-112">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="a151c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a151c-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a151c-114">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="a151c-114">Not applicable</span></span>  |
|<span data-ttu-id="a151c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a151c-115">Application</span></span> | <span data-ttu-id="a151c-116">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="a151c-116">User.Export.All and User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a151c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a151c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a151c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a151c-118">Request headers</span></span>
| <span data-ttu-id="a151c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a151c-119">Name</span></span>      |<span data-ttu-id="a151c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a151c-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a151c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a151c-121">Authorization</span></span>  | <span data-ttu-id="a151c-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="a151c-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a151c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a151c-123">Request body</span></span>
<span data-ttu-id="a151c-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a151c-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a151c-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="a151c-125">Response</span></span>
<span data-ttu-id="a151c-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [dataPolicyOperation](../resources/datapolicyoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a151c-126">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a151c-127">Пример</span><span class="sxs-lookup"><span data-stu-id="a151c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a151c-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="a151c-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a151c-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="a151c-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
# <a name="c"></a>[<span data-ttu-id="a151c-130">C#</span><span class="sxs-lookup"><span data-stu-id="a151c-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-datapolicyoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a151c-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a151c-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-datapolicyoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a151c-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a151c-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-datapolicyoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a151c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a151c-133">Response</span></span>
<span data-ttu-id="a151c-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a151c-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
