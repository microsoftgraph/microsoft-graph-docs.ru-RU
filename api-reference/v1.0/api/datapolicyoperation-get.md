---
title: Get dataPolicyOperation
description: Извлечение свойств объекта dataPolicyOperation.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 60284a0664c693168aa4279a1c48a6a6278d45eb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039799"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="91c0f-103">Get dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="91c0f-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="91c0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91c0f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="91c0f-105">Извлечение свойств **объекта dataPolicyOperation.**</span><span class="sxs-lookup"><span data-stu-id="91c0f-105">Retrieve the properties of a **dataPolicyOperation** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="91c0f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91c0f-106">Permissions</span></span>
<span data-ttu-id="91c0f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91c0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91c0f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91c0f-109">Permission type</span></span>      | <span data-ttu-id="91c0f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91c0f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91c0f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91c0f-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="91c0f-112">User.Export.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="91c0f-112">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="91c0f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91c0f-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="91c0f-114">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="91c0f-114">Not applicable</span></span>  |
|<span data-ttu-id="91c0f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91c0f-115">Application</span></span> | <span data-ttu-id="91c0f-116">User.Export.All, User.Read.All</span><span class="sxs-lookup"><span data-stu-id="91c0f-116">User.Export.All, User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="91c0f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91c0f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="91c0f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91c0f-118">Request headers</span></span>
| <span data-ttu-id="91c0f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="91c0f-119">Name</span></span>      |<span data-ttu-id="91c0f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="91c0f-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="91c0f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91c0f-121">Authorization</span></span>  | <span data-ttu-id="91c0f-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="91c0f-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="91c0f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91c0f-123">Request body</span></span>
<span data-ttu-id="91c0f-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91c0f-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="91c0f-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="91c0f-125">Response</span></span>
<span data-ttu-id="91c0f-126">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект dataPolicyOperation](../resources/datapolicyoperation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="91c0f-126">If successful, this method returns a `200 OK` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91c0f-127">Пример</span><span class="sxs-lookup"><span data-stu-id="91c0f-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91c0f-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="91c0f-128">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="91c0f-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="91c0f-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/dataPolicyOperations/{id}
```
# <a name="c"></a>[<span data-ttu-id="91c0f-130">C#</span><span class="sxs-lookup"><span data-stu-id="91c0f-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-datapolicyoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91c0f-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91c0f-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-datapolicyoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91c0f-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91c0f-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-datapolicyoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="91c0f-133">Java</span><span class="sxs-lookup"><span data-stu-id="91c0f-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-datapolicyoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="91c0f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="91c0f-134">Response</span></span>
><span data-ttu-id="91c0f-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="91c0f-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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

