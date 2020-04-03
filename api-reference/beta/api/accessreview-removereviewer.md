---
title: Удаление рецензента Акцессревиев
description: Удаление рецензента проверки доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 88a4fdcb6b50377c232c051e287681b0e41828ef
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123533"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="ae56a-103">Удаление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="ae56a-103">Remove accessReview reviewer</span></span>

<span data-ttu-id="ae56a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae56a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae56a-105">В функции [рецензирования Access](../resources/accessreviews-root.md) в Azure AD обновите существующий объект [акцессревиев](../resources/accessreview.md) , чтобы удалить пользователя в качестве проверяющего.</span><span class="sxs-lookup"><span data-stu-id="ae56a-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="ae56a-106">Эта операция разрешена только для проверки доступа, которая еще не завершена, и только для проверки доступа, в которой явно указаны рецензенты.</span><span class="sxs-lookup"><span data-stu-id="ae56a-106">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="ae56a-107">Эта операция не разрешена для проверки доступа, при которой пользователи просматривают собственный доступ, и не предназначены для проверки доступа, в которой владельцы группы назначаются в качестве проверяющих.</span><span class="sxs-lookup"><span data-stu-id="ae56a-107">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="ae56a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae56a-108">Permissions</span></span>
<span data-ttu-id="ae56a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae56a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae56a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae56a-111">Permission type</span></span>                        | <span data-ttu-id="ae56a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae56a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae56a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae56a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ae56a-114">Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ae56a-114">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="ae56a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae56a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae56a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae56a-116">Not supported.</span></span> |
|<span data-ttu-id="ae56a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae56a-117">Application</span></span>                            | <span data-ttu-id="ae56a-118">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="ae56a-118">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae56a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae56a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews/{reviewId}/reviewers/{userId}
```
## <a name="request-headers"></a><span data-ttu-id="ae56a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae56a-120">Request headers</span></span>
| <span data-ttu-id="ae56a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ae56a-121">Name</span></span>         | <span data-ttu-id="ae56a-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ae56a-122">Type</span></span>        | <span data-ttu-id="ae56a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ae56a-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="ae56a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae56a-124">Authorization</span></span> | <span data-ttu-id="ae56a-125">string</span><span class="sxs-lookup"><span data-stu-id="ae56a-125">string</span></span> | <span data-ttu-id="ae56a-p103">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae56a-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae56a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae56a-128">Request body</span></span>
<span data-ttu-id="ae56a-129">Не следует предоставлять текст запроса.</span><span class="sxs-lookup"><span data-stu-id="ae56a-129">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="ae56a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae56a-130">Response</span></span>
<span data-ttu-id="ae56a-131">В случае успешного выполнения этот метод возвращает код ответа серии 200.</span><span class="sxs-lookup"><span data-stu-id="ae56a-131">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="ae56a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ae56a-132">Example</span></span>

<span data-ttu-id="ae56a-133">В этом примере показано, как обновить доступ к одноразовой (не возможной) проверке доступа, чтобы удалить ненужного проверяющего.</span><span class="sxs-lookup"><span data-stu-id="ae56a-133">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="ae56a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae56a-134">Request</span></span>
<span data-ttu-id="ae56a-135">В URL-адресе запроса укажите идентификатор объекта Акцессревиев, а затем идентификатор объекта пользователя.</span><span class="sxs-lookup"><span data-stu-id="ae56a-135">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>


# <a name="http"></a>[<span data-ttu-id="ae56a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae56a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```
# <a name="c"></a>[<span data-ttu-id="ae56a-137">C#</span><span class="sxs-lookup"><span data-stu-id="ae56a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae56a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae56a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae56a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae56a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ae56a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae56a-140">Response</span></span>
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
