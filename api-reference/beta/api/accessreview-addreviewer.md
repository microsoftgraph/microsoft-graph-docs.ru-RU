---
title: Добавление рецензента Акцессревиев
description: 'В функции рецензирования Access в Azure AD обновите существующий объект Акцессревиев, чтобы добавить другого пользователя в качестве проверяющего.  Эта операция разрешена только для проверки доступа, которая еще не завершена, и только для проверки доступа, в которой явно указаны рецензенты. Эта операция не разрешена для проверки доступа, при которой пользователи просматривают собственный доступ, и не предназначены для проверки доступа, в которой владельцы группы назначаются в качестве проверяющих. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 08e5116c1948bc3cfafca0dc76232b8896d5e95c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440143"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="2c2e8-105">Добавление рецензента Акцессревиев</span><span class="sxs-lookup"><span data-stu-id="2c2e8-105">Add accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c2e8-106">В функции рецензирования [Access](../resources/accessreviews-root.md) в Azure AD обновите существующий объект [акцессревиев](../resources/accessreview.md) , чтобы добавить другого пользователя в качестве проверяющего.</span><span class="sxs-lookup"><span data-stu-id="2c2e8-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="2c2e8-107">Эта операция разрешена только для проверки доступа, которая еще не завершена, и только для проверки доступа, в которой явно указаны рецензенты.</span><span class="sxs-lookup"><span data-stu-id="2c2e8-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="2c2e8-108">Эта операция не разрешена для проверки доступа, при которой пользователи просматривают собственный доступ, и не предназначены для проверки доступа, в которой владельцы группы назначаются в качестве проверяющих.</span><span class="sxs-lookup"><span data-stu-id="2c2e8-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="2c2e8-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2c2e8-109">Permissions</span></span>
<span data-ttu-id="2c2e8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c2e8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c2e8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2c2e8-112">Permission type</span></span>                        | <span data-ttu-id="2c2e8-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2c2e8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c2e8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2c2e8-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c2e8-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c2e8-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="2c2e8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2c2e8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c2e8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c2e8-117">Not supported.</span></span> |
|<span data-ttu-id="2c2e8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2c2e8-118">Application</span></span>                            | <span data-ttu-id="2c2e8-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c2e8-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c2e8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2c2e8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="2c2e8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2c2e8-121">Request headers</span></span>
| <span data-ttu-id="2c2e8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2c2e8-122">Name</span></span>         | <span data-ttu-id="2c2e8-123">Тип</span><span class="sxs-lookup"><span data-stu-id="2c2e8-123">Type</span></span>        | <span data-ttu-id="2c2e8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2c2e8-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2c2e8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c2e8-125">Authorization</span></span> | <span data-ttu-id="2c2e8-126">string</span><span class="sxs-lookup"><span data-stu-id="2c2e8-126">string</span></span> | <span data-ttu-id="2c2e8-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2c2e8-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c2e8-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2c2e8-129">Request body</span></span>
<span data-ttu-id="2c2e8-130">В тексте запроса добавьте представление идентификатора пользователя, который будет рецензентом, в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c2e8-130">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="2c2e8-131">В следующей таблице приведены свойства, которые можно указать при обновлении Акцессревиев.</span><span class="sxs-lookup"><span data-stu-id="2c2e8-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="2c2e8-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c2e8-132">Property</span></span>     | <span data-ttu-id="2c2e8-133">Тип</span><span class="sxs-lookup"><span data-stu-id="2c2e8-133">Type</span></span>        | <span data-ttu-id="2c2e8-134">Описание</span><span class="sxs-lookup"><span data-stu-id="2c2e8-134">Description</span></span> |
|:-------------|:------------|:------------|
| `id`        | `String`   | <span data-ttu-id="2c2e8-135">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="2c2e8-135">The user ID.</span></span>|


## <a name="response"></a><span data-ttu-id="2c2e8-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c2e8-136">Response</span></span>
<span data-ttu-id="2c2e8-137">В случае успешного выполнения этот метод возвращает `201, Created` код отклика.</span><span class="sxs-lookup"><span data-stu-id="2c2e8-137">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="2c2e8-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2c2e8-138">Example</span></span>

<span data-ttu-id="2c2e8-139">В этом примере показано, как обновить доступ к одноразовой (неповторной) проверке доступа с помощью дополнительного проверяющего.</span><span class="sxs-lookup"><span data-stu-id="2c2e8-139">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="2c2e8-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="2c2e8-140">Request</span></span>
<span data-ttu-id="2c2e8-141">В тексте запроса добавьте представление идентификатора объекта пользователя в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c2e8-141">In the request body, supply a JSON representation of the id of the user object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2c2e8-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c2e8-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2c2e8-143">C#</span><span class="sxs-lookup"><span data-stu-id="2c2e8-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c2e8-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="2c2e8-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2c2e8-145">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2c2e8-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2c2e8-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2c2e8-146">Response</span></span>
><span data-ttu-id="2c2e8-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2c2e8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
