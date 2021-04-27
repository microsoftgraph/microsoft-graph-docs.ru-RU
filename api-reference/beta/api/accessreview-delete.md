---
title: Удаление accessReview
description: В функции обзоров доступа Azure AD удалите объект accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8877c0778f9924995c75dd47b331608d4994a62f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048507"
---
# <a name="delete-accessreview"></a><span data-ttu-id="64e68-103">Удаление accessReview</span><span class="sxs-lookup"><span data-stu-id="64e68-103">Delete accessReview</span></span>

<span data-ttu-id="64e68-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64e68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64e68-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) удалите [объект accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="64e68-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="64e68-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64e68-106">Permissions</span></span>
<span data-ttu-id="64e68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64e68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64e68-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64e68-109">Permission type</span></span>                        | <span data-ttu-id="64e68-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64e68-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="64e68-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64e68-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="64e68-112">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64e68-112">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="64e68-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64e68-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64e68-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64e68-114">Not supported.</span></span> |
|<span data-ttu-id="64e68-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="64e68-115">Application</span></span>                            | <span data-ttu-id="64e68-116">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="64e68-116">AccessReview.ReadWrite.Membership</span></span> |

<span data-ttu-id="64e68-117">Вызываемая должна также иметь разрешение ProgramControl.ReadWrite.All, чтобы удалить [программуControl](../resources/programcontrol.md).</span><span class="sxs-lookup"><span data-stu-id="64e68-117">The caller should also have ProgramControl.ReadWrite.All permission, so that it can delete a [programControl](../resources/programcontrol.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="64e68-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64e68-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews/{reviewId}
```
## <a name="request-headers"></a><span data-ttu-id="64e68-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64e68-119">Request headers</span></span>
| <span data-ttu-id="64e68-120">Имя</span><span class="sxs-lookup"><span data-stu-id="64e68-120">Name</span></span>         | <span data-ttu-id="64e68-121">Тип</span><span class="sxs-lookup"><span data-stu-id="64e68-121">Type</span></span>        | <span data-ttu-id="64e68-122">Описание</span><span class="sxs-lookup"><span data-stu-id="64e68-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="64e68-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64e68-123">Authorization</span></span> | <span data-ttu-id="64e68-124">string</span><span class="sxs-lookup"><span data-stu-id="64e68-124">string</span></span> | <span data-ttu-id="64e68-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64e68-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64e68-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64e68-127">Request body</span></span>
<span data-ttu-id="64e68-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64e68-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="64e68-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="64e68-129">Response</span></span>
<span data-ttu-id="64e68-p103">При успешном выполнении этот метод возвращает код отклика `204, No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="64e68-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64e68-132">Пример</span><span class="sxs-lookup"><span data-stu-id="64e68-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64e68-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="64e68-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="64e68-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="64e68-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/
```
# <a name="c"></a>[<span data-ttu-id="64e68-135">C#</span><span class="sxs-lookup"><span data-stu-id="64e68-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64e68-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64e68-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64e68-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64e68-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64e68-138">Java</span><span class="sxs-lookup"><span data-stu-id="64e68-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="64e68-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="64e68-139">Response</span></span>
><span data-ttu-id="64e68-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="64e68-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


