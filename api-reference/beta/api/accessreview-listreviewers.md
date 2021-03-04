---
title: Рецензенты списка accessReview
description: В функции обзоров доступа Azure AD извлекаем рецензентов объекта accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7d77ac50435a9923ec8e504a135e36c6b406f764
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439319"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="d3c42-103">Рецензенты списка accessReview</span><span class="sxs-lookup"><span data-stu-id="d3c42-103">List accessReview reviewers</span></span>

<span data-ttu-id="d3c42-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3c42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3c42-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) извлекаем рецензентов объекта [accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="d3c42-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d3c42-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3c42-106">Permissions</span></span>
<span data-ttu-id="d3c42-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3c42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3c42-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3c42-109">Permission type</span></span>                        | <span data-ttu-id="d3c42-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3c42-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3c42-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3c42-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3c42-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3c42-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="d3c42-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3c42-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3c42-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3c42-114">Not supported.</span></span> |
|<span data-ttu-id="d3c42-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d3c42-115">Application</span></span>                            | <span data-ttu-id="d3c42-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="d3c42-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |


 <span data-ttu-id="d3c42-117">Подписанный пользователь также должен быть в роли каталога, что позволяет им читать обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="d3c42-117">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="d3c42-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3c42-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="d3c42-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3c42-119">Request headers</span></span>
| <span data-ttu-id="d3c42-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d3c42-120">Name</span></span>         | <span data-ttu-id="d3c42-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d3c42-121">Type</span></span>        | <span data-ttu-id="d3c42-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d3c42-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d3c42-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3c42-123">Authorization</span></span> | <span data-ttu-id="d3c42-124">string</span><span class="sxs-lookup"><span data-stu-id="d3c42-124">string</span></span> | <span data-ttu-id="d3c42-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3c42-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3c42-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d3c42-127">Request body</span></span>
<span data-ttu-id="d3c42-128">Не следует поставлять тело запроса.</span><span class="sxs-lookup"><span data-stu-id="d3c42-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="d3c42-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3c42-129">Response</span></span>
<span data-ttu-id="d3c42-130">В случае успешной работы этот метод возвращает код отклика и массив объектов `200, OK` [userIdentity](../resources/useridentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d3c42-130">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3c42-131">Пример</span><span class="sxs-lookup"><span data-stu-id="d3c42-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3c42-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3c42-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d3c42-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3c42-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```
# <a name="c"></a>[<span data-ttu-id="d3c42-134">C#</span><span class="sxs-lookup"><span data-stu-id="d3c42-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-reviewers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3c42-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3c42-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-reviewers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3c42-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3c42-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-reviewers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3c42-137">Java</span><span class="sxs-lookup"><span data-stu-id="d3c42-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-reviewers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d3c42-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3c42-138">Response</span></span>
><span data-ttu-id="d3c42-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3c42-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userIdentity",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":
    [
        {
            "id":"006111db-0810-4494-a6df-904d368bd81b"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="d3c42-141">См. также</span><span class="sxs-lookup"><span data-stu-id="d3c42-141">See also</span></span>

| <span data-ttu-id="d3c42-142">Метод</span><span class="sxs-lookup"><span data-stu-id="d3c42-142">Method</span></span>           | <span data-ttu-id="d3c42-143">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d3c42-143">Return Type</span></span>    |<span data-ttu-id="d3c42-144">Описание</span><span class="sxs-lookup"><span data-stu-id="d3c42-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d3c42-145">Получить accessReview</span><span class="sxs-lookup"><span data-stu-id="d3c42-145">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="d3c42-146">accessReview</span><span class="sxs-lookup"><span data-stu-id="d3c42-146">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="d3c42-147">Извлечение обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="d3c42-147">Retrieve an access review.</span></span> |
|[<span data-ttu-id="d3c42-148">Добавление рецензента accessReview</span><span class="sxs-lookup"><span data-stu-id="d3c42-148">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="d3c42-149">Нет.</span><span class="sxs-lookup"><span data-stu-id="d3c42-149">None.</span></span>   |   <span data-ttu-id="d3c42-150">Добавление рецензента в accessReview.</span><span class="sxs-lookup"><span data-stu-id="d3c42-150">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="d3c42-151">Удаление рецензента accessReview</span><span class="sxs-lookup"><span data-stu-id="d3c42-151">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="d3c42-152">Нет.</span><span class="sxs-lookup"><span data-stu-id="d3c42-152">None.</span></span> |   <span data-ttu-id="d3c42-153">Удаление рецензента из accessReview.</span><span class="sxs-lookup"><span data-stu-id="d3c42-153">Remove a reviewer from an accessReview.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


