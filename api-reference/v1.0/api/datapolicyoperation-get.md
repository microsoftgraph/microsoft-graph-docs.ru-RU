---
title: Получение dataPolicyOperation
description: Получение свойств объекта dataPolicyOperation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 60dcf95b33de13b284f72ef06f3c2ea72a4a7409
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003009"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="81c69-103">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="81c69-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="81c69-104">Получение свойств объекта **dataPolicyOperation** .</span><span class="sxs-lookup"><span data-stu-id="81c69-104">Retrieve the properties of a **dataPolicyOperation** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="81c69-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81c69-105">Permissions</span></span>
<span data-ttu-id="81c69-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81c69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81c69-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81c69-108">Permission type</span></span>      | <span data-ttu-id="81c69-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81c69-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81c69-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81c69-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="81c69-111">User. Export. ALL, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="81c69-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="81c69-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81c69-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="81c69-113">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="81c69-113">Not applicable</span></span>  |
|<span data-ttu-id="81c69-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81c69-114">Application</span></span> | <span data-ttu-id="81c69-115">User. Export. ALL, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="81c69-115">User.Export.All, User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="81c69-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81c69-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="81c69-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81c69-117">Request headers</span></span>
| <span data-ttu-id="81c69-118">Имя</span><span class="sxs-lookup"><span data-stu-id="81c69-118">Name</span></span>      |<span data-ttu-id="81c69-119">Описание</span><span class="sxs-lookup"><span data-stu-id="81c69-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="81c69-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81c69-120">Authorization</span></span>  | <span data-ttu-id="81c69-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="81c69-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="81c69-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="81c69-122">Request body</span></span>
<span data-ttu-id="81c69-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="81c69-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="81c69-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="81c69-124">Response</span></span>
<span data-ttu-id="81c69-125">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [dataPolicyOperation](../resources/datapolicyoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="81c69-125">If successful, this method returns a `200 OK` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="81c69-126">Пример</span><span class="sxs-lookup"><span data-stu-id="81c69-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81c69-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="81c69-127">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="81c69-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="81c69-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/dataPolicyOperations/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="81c69-129">C#</span><span class="sxs-lookup"><span data-stu-id="81c69-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-datapolicyoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81c69-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="81c69-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-datapolicyoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="81c69-131">Цель — C</span><span class="sxs-lookup"><span data-stu-id="81c69-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-datapolicyoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="81c69-132">Java</span><span class="sxs-lookup"><span data-stu-id="81c69-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-datapolicyoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="81c69-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="81c69-133">Response</span></span>
><span data-ttu-id="81c69-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="81c69-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "progress": "double-value"
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
