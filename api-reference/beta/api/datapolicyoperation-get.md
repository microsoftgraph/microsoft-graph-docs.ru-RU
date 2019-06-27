---
title: Получение dataPolicyOperation
description: Получение свойств объекта dataPolicyOperation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: af51e3e0467ba59f588b27ac597a53e58f9e3b5c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261042"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="34f46-103">Получение dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="34f46-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="34f46-104">Получение свойств объекта dataPolicyOperation.</span><span class="sxs-lookup"><span data-stu-id="34f46-104">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="34f46-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34f46-105">Permissions</span></span>
<span data-ttu-id="34f46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34f46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34f46-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34f46-108">Permission type</span></span>      | <span data-ttu-id="34f46-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34f46-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34f46-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34f46-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="34f46-111">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="34f46-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="34f46-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34f46-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="34f46-113">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="34f46-113">Not applicable</span></span>  |
|<span data-ttu-id="34f46-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34f46-114">Application</span></span> | <span data-ttu-id="34f46-115">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="34f46-115">User.Export.All and User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="34f46-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34f46-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="34f46-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34f46-117">Request headers</span></span>
| <span data-ttu-id="34f46-118">Имя</span><span class="sxs-lookup"><span data-stu-id="34f46-118">Name</span></span>      |<span data-ttu-id="34f46-119">Описание</span><span class="sxs-lookup"><span data-stu-id="34f46-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="34f46-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34f46-120">Authorization</span></span>  | <span data-ttu-id="34f46-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="34f46-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="34f46-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="34f46-122">Request body</span></span>
<span data-ttu-id="34f46-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="34f46-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="34f46-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="34f46-124">Response</span></span>
<span data-ttu-id="34f46-125">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [dataPolicyOperation](../resources/datapolicyoperation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34f46-125">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="34f46-126">Пример</span><span class="sxs-lookup"><span data-stu-id="34f46-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34f46-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="34f46-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="34f46-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="34f46-128">Response</span></span>
<span data-ttu-id="34f46-p102">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34f46-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="34f46-131">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="34f46-131">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="34f46-132">C#</span><span class="sxs-lookup"><span data-stu-id="34f46-132">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_datapolicyoperation-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="34f46-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="34f46-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_datapolicyoperation-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="34f46-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="34f46-134">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_datapolicyoperation-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/datapolicyoperation-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/datapolicyoperation-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/datapolicyoperation-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
