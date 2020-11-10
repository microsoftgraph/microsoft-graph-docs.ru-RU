---
title: Создание Воркбуккомментрепли
description: Создание нового Воркбуккомментрепли.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: fb76b19dde2034d11b5491a78e883d009d34e70d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964334"
---
# <a name="create-workbookcommentreply"></a><span data-ttu-id="cba67-103">Создание Воркбуккомментрепли</span><span class="sxs-lookup"><span data-stu-id="cba67-103">Create workbookCommentReply</span></span>

<span data-ttu-id="cba67-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cba67-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cba67-105">Создание нового объекта [воркбуккомментрепли](../resources/workbookcommentreply.md) .</span><span class="sxs-lookup"><span data-stu-id="cba67-105">Create a new [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cba67-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cba67-106">Permissions</span></span>

<span data-ttu-id="cba67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cba67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cba67-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cba67-109">Permission type</span></span>                        | <span data-ttu-id="cba67-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cba67-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cba67-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cba67-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cba67-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cba67-112">Files.ReadWrite</span></span> |
| <span data-ttu-id="cba67-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cba67-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cba67-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cba67-114">Not supported.</span></span> |
| <span data-ttu-id="cba67-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cba67-115">Application</span></span>                            | <span data-ttu-id="cba67-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cba67-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cba67-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cba67-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /workbook/comments/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="cba67-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cba67-118">Request headers</span></span>

| <span data-ttu-id="cba67-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cba67-119">Name</span></span>          | <span data-ttu-id="cba67-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cba67-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cba67-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cba67-121">Authorization</span></span> | <span data-ttu-id="cba67-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cba67-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cba67-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cba67-124">Request body</span></span>

<span data-ttu-id="cba67-125">В тексте запроса добавьте представление объекта [воркбуккомментрепли](../resources/workbookcommentreply.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cba67-125">In the request body, supply a JSON representation of a [workbookCommentReply](../resources/workbookcommentreply.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cba67-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="cba67-126">Response</span></span>

<span data-ttu-id="cba67-127">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [воркбуккомментрепли](../resources/workbookcommentreply.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cba67-127">If successful, this method returns a `201 Created` response code and a new [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cba67-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="cba67-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cba67-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="cba67-129">Request</span></span>

<span data-ttu-id="cba67-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cba67-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cba67-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="cba67-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_workbookcommentreply_from_workbookcomment"
}-->

```http
POST https://graph.microsoft.com/beta/drive/items/{id}/workbook/comments/{id}/replies
Content-type: application/json

{
  "content": "This is my reply to the comment.",
  "contentType": "plain"
}
```
# <a name="c"></a>[<span data-ttu-id="cba67-132">C#</span><span class="sxs-lookup"><span data-stu-id="cba67-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workbookcommentreply-from-workbookcomment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cba67-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cba67-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workbookcommentreply-from-workbookcomment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cba67-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cba67-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workbookcommentreply-from-workbookcomment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cba67-135">Java</span><span class="sxs-lookup"><span data-stu-id="cba67-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-workbookcommentreply-from-workbookcomment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cba67-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="cba67-136">Response</span></span>

<span data-ttu-id="cba67-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cba67-137">The following is an example of the response.</span></span>

> <span data-ttu-id="cba67-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cba67-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookCommentReply"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "content": "This is my reply to the comment.",
  "contentType": "plain",
  "id": "{97A21473-8339-4BF0-BCB6-F55E4909FFB8}"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create workbookCommentReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


