---
title: Список рецензентов Акцессревиев
description: В функции рецензирования Access в Azure AD извлеките проверяющих объект Акцессревиев.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 756cb2d7bc93ea8fe490d0f857c609c3f82229f6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586004"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="85d21-103">Список рецензентов Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="85d21-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85d21-104">В функции рецензирования [Access](../resources/accessreviews-root.md) в Azure AD извлеките проверяющих объект [акцессревиев](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="85d21-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="85d21-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85d21-105">Permissions</span></span>
<span data-ttu-id="85d21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85d21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85d21-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85d21-108">Permission type</span></span>                        | <span data-ttu-id="85d21-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85d21-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="85d21-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85d21-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="85d21-111">Акцессревиев. Read. ALL, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="85d21-111">AccessReview.Read.All, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="85d21-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85d21-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85d21-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85d21-113">Not supported.</span></span> |
|<span data-ttu-id="85d21-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85d21-114">Application</span></span>                            | <span data-ttu-id="85d21-115">AccessReview.Read.All</span><span class="sxs-lookup"><span data-stu-id="85d21-115">AccessReview.Read.All</span></span>  |


 <span data-ttu-id="85d21-116">Пользователь, вошедшего в систему, также должен быть членом роли каталога, который позволяет им читать проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="85d21-116">The signed in user must also be in a directory role that permits them to read an access review.</span></span>

## <a name="http-request"></a><span data-ttu-id="85d21-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85d21-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="85d21-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85d21-118">Request headers</span></span>
| <span data-ttu-id="85d21-119">Имя</span><span class="sxs-lookup"><span data-stu-id="85d21-119">Name</span></span>         | <span data-ttu-id="85d21-120">Тип</span><span class="sxs-lookup"><span data-stu-id="85d21-120">Type</span></span>        | <span data-ttu-id="85d21-121">Описание</span><span class="sxs-lookup"><span data-stu-id="85d21-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="85d21-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="85d21-122">Authorization</span></span> | <span data-ttu-id="85d21-123">string</span><span class="sxs-lookup"><span data-stu-id="85d21-123">string</span></span> | <span data-ttu-id="85d21-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85d21-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85d21-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85d21-126">Request body</span></span>
<span data-ttu-id="85d21-127">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="85d21-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="85d21-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="85d21-128">Response</span></span>
<span data-ttu-id="85d21-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и массив объектов [userIdentity](../resources/useridentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85d21-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85d21-130">Пример</span><span class="sxs-lookup"><span data-stu-id="85d21-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85d21-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="85d21-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
```

##### <a name="response"></a><span data-ttu-id="85d21-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="85d21-132">Response</span></span>
><span data-ttu-id="85d21-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85d21-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="85d21-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="85d21-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="85d21-136">Языках</span><span class="sxs-lookup"><span data-stu-id="85d21-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview_reviewers-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="85d21-137">Язык</span><span class="sxs-lookup"><span data-stu-id="85d21-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview_reviewers-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="85d21-138">См. также</span><span class="sxs-lookup"><span data-stu-id="85d21-138">See also</span></span>

| <span data-ttu-id="85d21-139">Метод</span><span class="sxs-lookup"><span data-stu-id="85d21-139">Method</span></span>           | <span data-ttu-id="85d21-140">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="85d21-140">Return Type</span></span>    |<span data-ttu-id="85d21-141">Описание</span><span class="sxs-lookup"><span data-stu-id="85d21-141">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="85d21-142">Получение Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="85d21-142">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="85d21-143">Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="85d21-143">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="85d21-144">Получение проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="85d21-144">Retrieve an access review.</span></span> |
|[<span data-ttu-id="85d21-145">Добавление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="85d21-145">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="85d21-146">Нет.</span><span class="sxs-lookup"><span data-stu-id="85d21-146">None.</span></span>   |   <span data-ttu-id="85d21-147">Добавьте проверяющего в объект Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="85d21-147">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="85d21-148">Удаление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="85d21-148">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="85d21-149">Нет.</span><span class="sxs-lookup"><span data-stu-id="85d21-149">None.</span></span> |   <span data-ttu-id="85d21-150">Удаление проверяющего из Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="85d21-150">Remove a reviewer from an accessReview.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listreviewers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-listreviewers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
