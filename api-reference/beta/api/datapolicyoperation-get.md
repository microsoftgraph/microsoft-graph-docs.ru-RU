---
title: Получение dataPolicyOperation
description: Получение свойств объекта dataPolicyOperation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7f230ec987ebb574d741a25f388feef79e221ec3
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718298"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="2b249-103">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="2b249-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="2b249-104">Получение свойств объекта dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="2b249-104">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b249-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b249-105">Permissions</span></span>
<span data-ttu-id="2b249-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b249-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b249-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b249-108">Permission type</span></span>      | <span data-ttu-id="2b249-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b249-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b249-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b249-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="2b249-111">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="2b249-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="2b249-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b249-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2b249-113">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="2b249-113">Not applicable</span></span>  |
|<span data-ttu-id="2b249-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b249-114">Application</span></span> | <span data-ttu-id="2b249-115">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="2b249-115">User.Export.All and User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2b249-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b249-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2b249-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b249-117">Request headers</span></span>
| <span data-ttu-id="2b249-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2b249-118">Name</span></span>      |<span data-ttu-id="2b249-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2b249-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2b249-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b249-120">Authorization</span></span>  | <span data-ttu-id="2b249-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="2b249-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b249-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2b249-122">Request body</span></span>
<span data-ttu-id="2b249-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b249-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2b249-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b249-124">Response</span></span>
<span data-ttu-id="2b249-125">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [dataPolicyOperation](../resources/datapolicyoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b249-125">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b249-126">Пример</span><span class="sxs-lookup"><span data-stu-id="2b249-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b249-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b249-127">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2b249-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b249-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2b249-129">C#</span><span class="sxs-lookup"><span data-stu-id="2b249-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-datapolicyoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b249-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b249-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-datapolicyoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2b249-131">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2b249-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-datapolicyoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2b249-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b249-132">Response</span></span>
<span data-ttu-id="2b249-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b249-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
