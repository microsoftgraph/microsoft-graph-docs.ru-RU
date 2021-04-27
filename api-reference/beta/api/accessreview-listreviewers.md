---
title: Рецензенты списка accessReview
description: В функции обзоров доступа Azure AD извлекаем рецензентов объекта accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 457064b9dfa866d0d5bfe8285b495ecd3f8a4fe4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048465"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="b9c45-103">Рецензенты списка accessReview</span><span class="sxs-lookup"><span data-stu-id="b9c45-103">List accessReview reviewers</span></span>

<span data-ttu-id="b9c45-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9c45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9c45-105">В функции обзоров доступа Azure [AD](../resources/accessreviews-root.md) извлекаем рецензентов объекта [accessReview.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="b9c45-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b9c45-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9c45-106">Permissions</span></span>
<span data-ttu-id="b9c45-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9c45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9c45-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9c45-109">Permission type</span></span>                        | <span data-ttu-id="b9c45-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9c45-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9c45-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9c45-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9c45-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9c45-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="b9c45-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9c45-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9c45-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9c45-114">Not supported.</span></span> |
|<span data-ttu-id="b9c45-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b9c45-115">Application</span></span>                            | <span data-ttu-id="b9c45-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="b9c45-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |


 <span data-ttu-id="b9c45-117">Подписанный пользователь также должен быть в роли каталога, что позволяет им читать обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="b9c45-117">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="b9c45-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9c45-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="b9c45-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9c45-119">Request headers</span></span>
| <span data-ttu-id="b9c45-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b9c45-120">Name</span></span>         | <span data-ttu-id="b9c45-121">Тип</span><span class="sxs-lookup"><span data-stu-id="b9c45-121">Type</span></span>        | <span data-ttu-id="b9c45-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b9c45-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b9c45-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9c45-123">Authorization</span></span> | <span data-ttu-id="b9c45-124">string</span><span class="sxs-lookup"><span data-stu-id="b9c45-124">string</span></span> | <span data-ttu-id="b9c45-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9c45-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9c45-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b9c45-127">Request body</span></span>
<span data-ttu-id="b9c45-128">Не следует поставлять тело запроса.</span><span class="sxs-lookup"><span data-stu-id="b9c45-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="b9c45-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9c45-129">Response</span></span>
<span data-ttu-id="b9c45-130">В случае успешной работы этот метод возвращает код отклика и массив объектов `200, OK` [userIdentity](../resources/useridentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b9c45-130">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9c45-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b9c45-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9c45-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9c45-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b9c45-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9c45-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```
# <a name="c"></a>[<span data-ttu-id="b9c45-134">C#</span><span class="sxs-lookup"><span data-stu-id="b9c45-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-reviewers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9c45-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9c45-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-reviewers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9c45-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9c45-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-reviewers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9c45-137">Java</span><span class="sxs-lookup"><span data-stu-id="b9c45-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-reviewers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b9c45-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9c45-138">Response</span></span>
><span data-ttu-id="b9c45-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b9c45-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="b9c45-140">См. также</span><span class="sxs-lookup"><span data-stu-id="b9c45-140">See also</span></span>

| <span data-ttu-id="b9c45-141">Метод</span><span class="sxs-lookup"><span data-stu-id="b9c45-141">Method</span></span>           | <span data-ttu-id="b9c45-142">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b9c45-142">Return Type</span></span>    |<span data-ttu-id="b9c45-143">Описание</span><span class="sxs-lookup"><span data-stu-id="b9c45-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b9c45-144">Получить accessReview</span><span class="sxs-lookup"><span data-stu-id="b9c45-144">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="b9c45-145">accessReview</span><span class="sxs-lookup"><span data-stu-id="b9c45-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="b9c45-146">Извлечение обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="b9c45-146">Retrieve an access review.</span></span> |
|[<span data-ttu-id="b9c45-147">Добавление рецензента accessReview</span><span class="sxs-lookup"><span data-stu-id="b9c45-147">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="b9c45-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b9c45-148">None.</span></span>   |   <span data-ttu-id="b9c45-149">Добавление рецензента в accessReview.</span><span class="sxs-lookup"><span data-stu-id="b9c45-149">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="b9c45-150">Удаление рецензента accessReview</span><span class="sxs-lookup"><span data-stu-id="b9c45-150">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="b9c45-151">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b9c45-151">None.</span></span> |   <span data-ttu-id="b9c45-152">Удаление рецензента из accessReview.</span><span class="sxs-lookup"><span data-stu-id="b9c45-152">Remove a reviewer from an accessReview.</span></span> |


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


