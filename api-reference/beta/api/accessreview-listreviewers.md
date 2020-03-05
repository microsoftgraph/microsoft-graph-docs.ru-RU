---
title: Список рецензентов Акцессревиев
description: В функции рецензирования Access в Azure AD извлеките проверяющих объект Акцессревиев.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 114a59e0d5e96983a30afcf31d8452c979f2f486
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441881"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="4ca5a-103">Список рецензентов Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="4ca5a-103">List accessReview reviewers</span></span>

<span data-ttu-id="4ca5a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4ca5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ca5a-105">В функции [рецензирования Access](../resources/accessreviews-root.md) в Azure AD извлеките проверяющих объект [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="4ca5a-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4ca5a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ca5a-106">Permissions</span></span>
<span data-ttu-id="4ca5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ca5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ca5a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ca5a-109">Permission type</span></span>                        | <span data-ttu-id="4ca5a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ca5a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ca5a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ca5a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ca5a-112">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4ca5a-112">AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="4ca5a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ca5a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ca5a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ca5a-114">Not supported.</span></span> |
|<span data-ttu-id="4ca5a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ca5a-115">Application</span></span>                            | <span data-ttu-id="4ca5a-116">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="4ca5a-116">AccessReview.Read.All, AccessReview.ReadWrite.Membership</span></span>  |


 <span data-ttu-id="4ca5a-117">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="4ca5a-117">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="4ca5a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ca5a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="4ca5a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ca5a-119">Request headers</span></span>
| <span data-ttu-id="4ca5a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4ca5a-120">Name</span></span>         | <span data-ttu-id="4ca5a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="4ca5a-121">Type</span></span>        | <span data-ttu-id="4ca5a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4ca5a-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4ca5a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ca5a-123">Authorization</span></span> | <span data-ttu-id="4ca5a-124">string</span><span class="sxs-lookup"><span data-stu-id="4ca5a-124">string</span></span> | <span data-ttu-id="4ca5a-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ca5a-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ca5a-127">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ca5a-127">Request body</span></span>
<span data-ttu-id="4ca5a-128">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="4ca5a-128">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="4ca5a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ca5a-129">Response</span></span>
<span data-ttu-id="4ca5a-130">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [userIdentity](../resources/useridentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4ca5a-130">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ca5a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4ca5a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ca5a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ca5a-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4ca5a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ca5a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```
# <a name="c"></a>[<span data-ttu-id="4ca5a-134">C#</span><span class="sxs-lookup"><span data-stu-id="4ca5a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-reviewers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ca5a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ca5a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-reviewers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ca5a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ca5a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-reviewers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4ca5a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ca5a-137">Response</span></span>
><span data-ttu-id="4ca5a-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4ca5a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4ca5a-140">См. также</span><span class="sxs-lookup"><span data-stu-id="4ca5a-140">See also</span></span>

| <span data-ttu-id="4ca5a-141">Метод</span><span class="sxs-lookup"><span data-stu-id="4ca5a-141">Method</span></span>           | <span data-ttu-id="4ca5a-142">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4ca5a-142">Return Type</span></span>    |<span data-ttu-id="4ca5a-143">Описание</span><span class="sxs-lookup"><span data-stu-id="4ca5a-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4ca5a-144">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="4ca5a-144">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="4ca5a-145">акцессревиев</span><span class="sxs-lookup"><span data-stu-id="4ca5a-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="4ca5a-146">Получение проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="4ca5a-146">Retrieve an access review.</span></span> |
|[<span data-ttu-id="4ca5a-147">Добавление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="4ca5a-147">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="4ca5a-148">Нет.</span><span class="sxs-lookup"><span data-stu-id="4ca5a-148">None.</span></span>   |   <span data-ttu-id="4ca5a-149">Добавьте проверяющего в объект Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="4ca5a-149">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="4ca5a-150">Удаление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="4ca5a-150">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="4ca5a-151">Нет.</span><span class="sxs-lookup"><span data-stu-id="4ca5a-151">None.</span></span> |   <span data-ttu-id="4ca5a-152">Удаление проверяющего из Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="4ca5a-152">Remove a reviewer from an accessReview.</span></span> |


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
