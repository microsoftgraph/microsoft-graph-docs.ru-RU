---
title: Получение dataPolicyOperation
description: Получение свойств объекта dataPolicyOperation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2ce26de4e8dadd58d7a3a337b1c8217d3db1d5eb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436120"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="c4cb5-103">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="c4cb5-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="c4cb5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c4cb5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c4cb5-105">Получение свойств объекта dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="c4cb5-105">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4cb5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4cb5-106">Permissions</span></span>
<span data-ttu-id="c4cb5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4cb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4cb5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4cb5-109">Permission type</span></span>      | <span data-ttu-id="c4cb5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4cb5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4cb5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4cb5-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="c4cb5-112">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="c4cb5-112">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="c4cb5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4cb5-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c4cb5-114">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="c4cb5-114">Not applicable</span></span>  |
|<span data-ttu-id="c4cb5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4cb5-115">Application</span></span> | <span data-ttu-id="c4cb5-116">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="c4cb5-116">User.Export.All and User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c4cb5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4cb5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c4cb5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4cb5-118">Request headers</span></span>
| <span data-ttu-id="c4cb5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c4cb5-119">Name</span></span>      |<span data-ttu-id="c4cb5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c4cb5-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c4cb5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4cb5-121">Authorization</span></span>  | <span data-ttu-id="c4cb5-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="c4cb5-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4cb5-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4cb5-123">Request body</span></span>
<span data-ttu-id="c4cb5-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c4cb5-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c4cb5-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4cb5-125">Response</span></span>
<span data-ttu-id="c4cb5-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [dataPolicyOperation](../resources/datapolicyoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c4cb5-126">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c4cb5-127">Пример</span><span class="sxs-lookup"><span data-stu-id="c4cb5-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4cb5-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4cb5-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c4cb5-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4cb5-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
# <a name="c"></a>[<span data-ttu-id="c4cb5-130">C#</span><span class="sxs-lookup"><span data-stu-id="c4cb5-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-datapolicyoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4cb5-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4cb5-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-datapolicyoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4cb5-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4cb5-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-datapolicyoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c4cb5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4cb5-133">Response</span></span>
<span data-ttu-id="c4cb5-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4cb5-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
