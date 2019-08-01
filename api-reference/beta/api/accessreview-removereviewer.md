---
title: Удаление рецензента Акцессревиев
description: 'В функции рецензирования Access в Azure AD обновите существующий объект Акцессревиев, чтобы удалить пользователя в качестве проверяющего.  Эта операция разрешена только для проверки доступа, которая еще не завершена, и только для проверки доступа, в которой явно указаны рецензенты. Эта операция не разрешена для проверки доступа, при которой пользователи просматривают собственный доступ, и не предназначены для проверки доступа, в которой владельцы группы назначаются в качестве проверяющих. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ddf8d2df743a3c3700dfed09016fd76dda37f714
ms.sourcegitcommit: a700f1c283a5d847cd1697e26bcd47bc8625384e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2019
ms.locfileid: "36049577"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="d6873-105">Удаление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="d6873-105">Remove accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6873-106">В функции рецензирования [Access](../resources/accessreviews-root.md) в Azure AD обновите существующий объект [акцессревиев](../resources/accessreview.md) , чтобы удалить пользователя в качестве проверяющего.</span><span class="sxs-lookup"><span data-stu-id="d6873-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="d6873-107">Эта операция разрешена только для проверки доступа, которая еще не завершена, и только для проверки доступа, в которой явно указаны рецензенты.</span><span class="sxs-lookup"><span data-stu-id="d6873-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="d6873-108">Эта операция не разрешена для проверки доступа, при которой пользователи просматривают собственный доступ, и не предназначены для проверки доступа, в которой владельцы группы назначаются в качестве проверяющих.</span><span class="sxs-lookup"><span data-stu-id="d6873-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="d6873-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6873-109">Permissions</span></span>
<span data-ttu-id="d6873-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6873-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6873-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6873-112">Permission type</span></span>                        | <span data-ttu-id="d6873-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6873-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6873-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6873-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6873-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6873-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="d6873-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6873-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6873-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6873-117">Not supported.</span></span> |
|<span data-ttu-id="d6873-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6873-118">Application</span></span>                            | <span data-ttu-id="d6873-119">Акцессревиев. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="d6873-119">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6873-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6873-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a><span data-ttu-id="d6873-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6873-121">Request headers</span></span>
| <span data-ttu-id="d6873-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d6873-122">Name</span></span>         | <span data-ttu-id="d6873-123">Тип</span><span class="sxs-lookup"><span data-stu-id="d6873-123">Type</span></span>        | <span data-ttu-id="d6873-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d6873-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d6873-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6873-125">Authorization</span></span> | <span data-ttu-id="d6873-126">string</span><span class="sxs-lookup"><span data-stu-id="d6873-126">string</span></span> | <span data-ttu-id="d6873-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6873-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6873-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d6873-129">Request body</span></span>
<span data-ttu-id="d6873-130">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="d6873-130">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="d6873-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6873-131">Response</span></span>
<span data-ttu-id="d6873-132">В случае успешного выполнения этот метод возвращает код ответа серии 200.</span><span class="sxs-lookup"><span data-stu-id="d6873-132">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="d6873-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d6873-133">Example</span></span>

<span data-ttu-id="d6873-134">В этом примере показано, как обновить доступ к одноразовой (не возможной) проверке доступа, чтобы удалить ненужного проверяющего.</span><span class="sxs-lookup"><span data-stu-id="d6873-134">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="d6873-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6873-135">Request</span></span>
<span data-ttu-id="d6873-136">В URL-адресе запроса укажите идентификатор объекта Акцессревиев, а затем идентификатор объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6873-136">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d6873-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6873-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d6873-138">C#</span><span class="sxs-lookup"><span data-stu-id="d6873-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6873-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="d6873-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d6873-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d6873-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d6873-141">Java</span><span class="sxs-lookup"><span data-stu-id="d6873-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-accessreview-reviewer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d6873-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6873-142">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
