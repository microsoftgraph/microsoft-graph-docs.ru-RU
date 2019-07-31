---
title: Список рецензентов Акцессревиев
description: В функции рецензирования Access в Azure AD извлеките проверяющих объект Акцессревиев.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d32abb41313a9008e6b222119a9b4d7a95553b0f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945993"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="fc518-103">Список рецензентов Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="fc518-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc518-104">В функции рецензирования [Access](../resources/accessreviews-root.md) в Azure AD извлеките проверяющих объект [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="fc518-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc518-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc518-105">Permissions</span></span>
<span data-ttu-id="fc518-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc518-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc518-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc518-108">Permission type</span></span>                        | <span data-ttu-id="fc518-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc518-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc518-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc518-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc518-111">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="fc518-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="fc518-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc518-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc518-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc518-113">Not supported.</span></span> |
|<span data-ttu-id="fc518-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc518-114">Application</span></span>                            | <span data-ttu-id="fc518-115">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc518-115">AccessReview.Read.All</span></span>  |


 <span data-ttu-id="fc518-116">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="fc518-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="fc518-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc518-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="fc518-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc518-118">Request headers</span></span>
| <span data-ttu-id="fc518-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fc518-119">Name</span></span>         | <span data-ttu-id="fc518-120">Тип</span><span class="sxs-lookup"><span data-stu-id="fc518-120">Type</span></span>        | <span data-ttu-id="fc518-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fc518-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fc518-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc518-122">Authorization</span></span> | <span data-ttu-id="fc518-123">string</span><span class="sxs-lookup"><span data-stu-id="fc518-123">string</span></span> | <span data-ttu-id="fc518-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fc518-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc518-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fc518-126">Request body</span></span>
<span data-ttu-id="fc518-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="fc518-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="fc518-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc518-128">Response</span></span>
<span data-ttu-id="fc518-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [userIdentity](../resources/useridentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc518-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc518-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fc518-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc518-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc518-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fc518-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc518-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fc518-133">C#</span><span class="sxs-lookup"><span data-stu-id="fc518-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-reviewers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc518-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="fc518-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-reviewers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fc518-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fc518-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-reviewers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fc518-136">Java</span><span class="sxs-lookup"><span data-stu-id="fc518-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-reviewers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fc518-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc518-137">Response</span></span>
><span data-ttu-id="fc518-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc518-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="fc518-140">См. также</span><span class="sxs-lookup"><span data-stu-id="fc518-140">See also</span></span>

| <span data-ttu-id="fc518-141">Метод</span><span class="sxs-lookup"><span data-stu-id="fc518-141">Method</span></span>           | <span data-ttu-id="fc518-142">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fc518-142">Return Type</span></span>    |<span data-ttu-id="fc518-143">Описание</span><span class="sxs-lookup"><span data-stu-id="fc518-143">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fc518-144">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="fc518-144">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="fc518-145">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="fc518-145">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="fc518-146">Получение проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="fc518-146">Retrieve an access review.</span></span> |
|[<span data-ttu-id="fc518-147">Добавление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="fc518-147">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="fc518-148">Нет.</span><span class="sxs-lookup"><span data-stu-id="fc518-148">None.</span></span>   |   <span data-ttu-id="fc518-149">Добавьте проверяющего в объект Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="fc518-149">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="fc518-150">Удаление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="fc518-150">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="fc518-151">Нет.</span><span class="sxs-lookup"><span data-stu-id="fc518-151">None.</span></span> |   <span data-ttu-id="fc518-152">Удаление проверяющего из Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="fc518-152">Remove a reviewer from an accessReview.</span></span> |


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
