---
title: Получение dataPolicyOperation
description: Получение свойств объекта dataPolicyOperation.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 749f9e62536949e4e74077640076337f7d8a5263
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591046"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="df7ae-103">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="df7ae-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="df7ae-104">Получение свойств объекта dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="df7ae-104">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="df7ae-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df7ae-105">Permissions</span></span>
<span data-ttu-id="df7ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df7ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df7ae-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df7ae-108">Permission type</span></span>      | <span data-ttu-id="df7ae-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df7ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df7ae-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df7ae-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="df7ae-111">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="df7ae-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="df7ae-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df7ae-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="df7ae-113">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="df7ae-113">Not applicable</span></span>  |
|<span data-ttu-id="df7ae-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df7ae-114">Application</span></span> | <span data-ttu-id="df7ae-115">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="df7ae-115">User.Export.All and User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="df7ae-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df7ae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="df7ae-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df7ae-117">Request headers</span></span>
| <span data-ttu-id="df7ae-118">Имя</span><span class="sxs-lookup"><span data-stu-id="df7ae-118">Name</span></span>      |<span data-ttu-id="df7ae-119">Описание</span><span class="sxs-lookup"><span data-stu-id="df7ae-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="df7ae-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="df7ae-120">Authorization</span></span>  | <span data-ttu-id="df7ae-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="df7ae-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="df7ae-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df7ae-122">Request body</span></span>
<span data-ttu-id="df7ae-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="df7ae-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="df7ae-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="df7ae-124">Response</span></span>
<span data-ttu-id="df7ae-125">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [dataPolicyOperation](../resources/datapolicyoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="df7ae-125">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="df7ae-126">Пример</span><span class="sxs-lookup"><span data-stu-id="df7ae-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df7ae-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="df7ae-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="df7ae-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="df7ae-128">Response</span></span>
<span data-ttu-id="df7ae-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df7ae-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="df7ae-131">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="df7ae-131">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="df7ae-132">Языках</span><span class="sxs-lookup"><span data-stu-id="df7ae-132">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_datapolicyoperation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="df7ae-133">Язык</span><span class="sxs-lookup"><span data-stu-id="df7ae-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_datapolicyoperation-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get dataPolicyOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/datapolicyoperation-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/datapolicyoperation-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
