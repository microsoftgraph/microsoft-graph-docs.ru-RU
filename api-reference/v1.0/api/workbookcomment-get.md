---
title: Получение Воркбуккоммент
description: Получение свойств и связей объекта воркбуккоммент.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 99e285fb127f38737cf611aa297691946cf054cb
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/11/2019
ms.locfileid: "36839159"
---
# <a name="get-workbookcomment"></a><span data-ttu-id="0bbb9-103">Получение Воркбуккоммент</span><span class="sxs-lookup"><span data-stu-id="0bbb9-103">Get workbookComment</span></span>

<span data-ttu-id="0bbb9-104">Получение свойств и связей объекта [воркбуккоммент](../resources/workbookcomment.md) .</span><span class="sxs-lookup"><span data-stu-id="0bbb9-104">Retrieve the properties and relationships of a [workbookComment](../resources/workbookcomment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0bbb9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0bbb9-105">Permissions</span></span>

<span data-ttu-id="0bbb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bbb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0bbb9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0bbb9-108">Permission type</span></span>                        | <span data-ttu-id="0bbb9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0bbb9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0bbb9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0bbb9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0bbb9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0bbb9-111">Files.ReadWrite</span></span> |
| <span data-ttu-id="0bbb9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0bbb9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bbb9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bbb9-113">Not supported.</span></span> |
| <span data-ttu-id="0bbb9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0bbb9-114">Application</span></span>                            | <span data-ttu-id="0bbb9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bbb9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bbb9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0bbb9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET workbook/comments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0bbb9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0bbb9-117">Request headers</span></span>

| <span data-ttu-id="0bbb9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0bbb9-118">Name</span></span>      |<span data-ttu-id="0bbb9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0bbb9-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0bbb9-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0bbb9-120">Authorization</span></span> | <span data-ttu-id="0bbb9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0bbb9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0bbb9-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0bbb9-123">Request body</span></span>

<span data-ttu-id="0bbb9-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0bbb9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bbb9-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bbb9-125">Response</span></span>

<span data-ttu-id="0bbb9-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [воркбуккоммент](../resources/workbookcomment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0bbb9-126">If successful, this method returns a `200 OK` response code and the requested [workbookComment](../resources/workbookcomment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0bbb9-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="0bbb9-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0bbb9-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bbb9-128">Request</span></span>

<span data-ttu-id="0bbb9-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0bbb9-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0bbb9-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0bbb9-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workbookcomment"
}-->

```http
GET https://graph.microsoft.com/v1.0/drive/root/workbook/comments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0bbb9-131">C#</span><span class="sxs-lookup"><span data-stu-id="0bbb9-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workbookcomment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0bbb9-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0bbb9-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workbookcomment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0bbb9-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0bbb9-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workbookcomment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0bbb9-134">Java</span><span class="sxs-lookup"><span data-stu-id="0bbb9-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workbookcomment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0bbb9-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bbb9-135">Response</span></span>

<span data-ttu-id="0bbb9-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0bbb9-136">The following is an example of the response.</span></span>

> <span data-ttu-id="0bbb9-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0bbb9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookComment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "content": "This is my comment.",
  "contentType": "plain",
  "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workbookComment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
