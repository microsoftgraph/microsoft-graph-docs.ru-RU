---
title: Добавление рецензента Акцессревиев
description: 'В функции рецензирования Access в Azure AD обновите существующий объект Акцессревиев, чтобы добавить другого пользователя в качестве проверяющего.  Эта операция разрешена только для проверки доступа, которая еще не завершена, и только для проверки доступа, в которой явно указаны рецензенты. Эта операция не разрешена для проверки доступа, при которой пользователи просматривают собственный доступ, и не предназначены для проверки доступа, в которой владельцы группы назначаются в качестве проверяющих. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aa8550e248bd34baf8d09c7ec72ced8cb9f578b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441933"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="0d61c-105">Добавление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="0d61c-105">Add accessReview reviewer</span></span>

<span data-ttu-id="0d61c-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0d61c-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d61c-107">В функции [рецензирования Access](../resources/accessreviews-root.md) в Azure AD обновите существующий объект [акцессревиев](../resources/accessreview.md) , чтобы добавить другого пользователя в качестве проверяющего.</span><span class="sxs-lookup"><span data-stu-id="0d61c-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="0d61c-108">Эта операция разрешена только для проверки доступа, которая еще не завершена, и только для проверки доступа, в которой явно указаны рецензенты.</span><span class="sxs-lookup"><span data-stu-id="0d61c-108">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="0d61c-109">Эта операция не разрешена для проверки доступа, при которой пользователи просматривают собственный доступ, и не предназначены для проверки доступа, в которой владельцы группы назначаются в качестве проверяющих.</span><span class="sxs-lookup"><span data-stu-id="0d61c-109">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="0d61c-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0d61c-110">Permissions</span></span>
<span data-ttu-id="0d61c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d61c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d61c-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d61c-113">Permission type</span></span>                        | <span data-ttu-id="0d61c-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d61c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d61c-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d61c-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d61c-116">Акцессревиев. ReadWrite. Membership, Акцессревиев. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0d61c-116">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="0d61c-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d61c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d61c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d61c-118">Not supported.</span></span> |
|<span data-ttu-id="0d61c-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d61c-119">Application</span></span>                            | <span data-ttu-id="0d61c-120">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="0d61c-120">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d61c-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d61c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="0d61c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d61c-122">Request headers</span></span>
| <span data-ttu-id="0d61c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="0d61c-123">Name</span></span>         | <span data-ttu-id="0d61c-124">Тип</span><span class="sxs-lookup"><span data-stu-id="0d61c-124">Type</span></span>        | <span data-ttu-id="0d61c-125">Описание</span><span class="sxs-lookup"><span data-stu-id="0d61c-125">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0d61c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d61c-126">Authorization</span></span> | <span data-ttu-id="0d61c-127">string</span><span class="sxs-lookup"><span data-stu-id="0d61c-127">string</span></span> | <span data-ttu-id="0d61c-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d61c-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d61c-130">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="0d61c-130">Request body</span></span>
<span data-ttu-id="0d61c-131">В тексте запроса добавьте представление идентификатора пользователя, который будет рецензентом, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d61c-131">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="0d61c-132">В следующей таблице приведены свойства, которые можно указать при обновлении Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="0d61c-132">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="0d61c-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d61c-133">Property</span></span>     | <span data-ttu-id="0d61c-134">Тип</span><span class="sxs-lookup"><span data-stu-id="0d61c-134">Type</span></span>        | <span data-ttu-id="0d61c-135">Описание</span><span class="sxs-lookup"><span data-stu-id="0d61c-135">Description</span></span> |
|:-------------|:------------|:------------|
| `id`        | `String`   | <span data-ttu-id="0d61c-136">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d61c-136">The user ID.</span></span>|


## <a name="response"></a><span data-ttu-id="0d61c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d61c-137">Response</span></span>
<span data-ttu-id="0d61c-138">В случае успешного выполнения этот метод возвращает `201, Created` код отклика.</span><span class="sxs-lookup"><span data-stu-id="0d61c-138">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="0d61c-139">Пример</span><span class="sxs-lookup"><span data-stu-id="0d61c-139">Example</span></span>

<span data-ttu-id="0d61c-140">В этом примере показано, как обновить доступ к одноразовой (неповторной) проверке доступа с помощью дополнительного проверяющего.</span><span class="sxs-lookup"><span data-stu-id="0d61c-140">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="0d61c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d61c-141">Request</span></span>
<span data-ttu-id="0d61c-142">В тексте запроса добавьте представление идентификатора объекта пользователя в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d61c-142">In the request body, supply a JSON representation of the id of the user object.</span></span>


# <a name="http"></a>[<span data-ttu-id="0d61c-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d61c-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
Content-Type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```
# <a name="c"></a>[<span data-ttu-id="0d61c-144">C#</span><span class="sxs-lookup"><span data-stu-id="0d61c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d61c-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d61c-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d61c-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d61c-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0d61c-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d61c-147">Response</span></span>
><span data-ttu-id="0d61c-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d61c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!--
{
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
