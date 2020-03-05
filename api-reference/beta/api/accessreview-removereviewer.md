---
title: Удаление рецензента Акцессревиев
description: 'В функции рецензирования Access в Azure AD обновите существующий объект Акцессревиев, чтобы удалить пользователя в качестве проверяющего.  Эта операция разрешена только для проверки доступа, которая еще не завершена, и только для проверки доступа, в которой явно указаны рецензенты. Эта операция не разрешена для проверки доступа, при которой пользователи просматривают собственный доступ, и не предназначены для проверки доступа, в которой владельцы группы назначаются в качестве проверяющих. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f81f7b4befc99ad457d570e5e66a2ce97bfe4ce2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441874"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="40d9d-105">Удаление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="40d9d-105">Remove accessReview reviewer</span></span>

<span data-ttu-id="40d9d-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="40d9d-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40d9d-107">В функции [рецензирования Access](../resources/accessreviews-root.md) в Azure AD обновите существующий объект [акцессревиев](../resources/accessreview.md) , чтобы удалить пользователя в качестве проверяющего.</span><span class="sxs-lookup"><span data-stu-id="40d9d-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="40d9d-108">Эта операция разрешена только для проверки доступа, которая еще не завершена, и только для проверки доступа, в которой явно указаны рецензенты.</span><span class="sxs-lookup"><span data-stu-id="40d9d-108">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="40d9d-109">Эта операция не разрешена для проверки доступа, при которой пользователи просматривают собственный доступ, и не предназначены для проверки доступа, в которой владельцы группы назначаются в качестве проверяющих.</span><span class="sxs-lookup"><span data-stu-id="40d9d-109">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="40d9d-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40d9d-110">Permissions</span></span>
<span data-ttu-id="40d9d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40d9d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40d9d-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40d9d-113">Permission type</span></span>                        | <span data-ttu-id="40d9d-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40d9d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="40d9d-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40d9d-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="40d9d-116">Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="40d9d-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="40d9d-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40d9d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40d9d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40d9d-118">Not supported.</span></span> |
|<span data-ttu-id="40d9d-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40d9d-119">Application</span></span>                            | <span data-ttu-id="40d9d-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="40d9d-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="40d9d-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40d9d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews/{reviewId}/reviewers/{userId}
```
## <a name="request-headers"></a><span data-ttu-id="40d9d-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40d9d-122">Request headers</span></span>
| <span data-ttu-id="40d9d-123">Имя</span><span class="sxs-lookup"><span data-stu-id="40d9d-123">Name</span></span>         | <span data-ttu-id="40d9d-124">Тип</span><span class="sxs-lookup"><span data-stu-id="40d9d-124">Type</span></span>        | <span data-ttu-id="40d9d-125">Описание</span><span class="sxs-lookup"><span data-stu-id="40d9d-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="40d9d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="40d9d-126">Authorization</span></span> | <span data-ttu-id="40d9d-127">string</span><span class="sxs-lookup"><span data-stu-id="40d9d-127">string</span></span> | <span data-ttu-id="40d9d-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40d9d-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40d9d-130">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="40d9d-130">Request body</span></span>
<span data-ttu-id="40d9d-131">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="40d9d-131">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="40d9d-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="40d9d-132">Response</span></span>
<span data-ttu-id="40d9d-133">В случае успешного выполнения этот метод возвращает код ответа серии 200.</span><span class="sxs-lookup"><span data-stu-id="40d9d-133">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="40d9d-134">Пример</span><span class="sxs-lookup"><span data-stu-id="40d9d-134">Example</span></span>

<span data-ttu-id="40d9d-135">В этом примере показано, как обновить доступ к одноразовой (не возможной) проверке доступа, чтобы удалить ненужного проверяющего.</span><span class="sxs-lookup"><span data-stu-id="40d9d-135">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="40d9d-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="40d9d-136">Request</span></span>
<span data-ttu-id="40d9d-137">В URL-адресе запроса укажите идентификатор объекта Акцессревиев, а затем идентификатор объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="40d9d-137">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>


# <a name="http"></a>[<span data-ttu-id="40d9d-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="40d9d-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```
# <a name="c"></a>[<span data-ttu-id="40d9d-139">C#</span><span class="sxs-lookup"><span data-stu-id="40d9d-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40d9d-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40d9d-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40d9d-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40d9d-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="40d9d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="40d9d-142">Response</span></span>
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
