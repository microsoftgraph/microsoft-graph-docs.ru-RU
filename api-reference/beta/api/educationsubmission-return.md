---
title: 'educationSubmission: Return'
description: Это действие делает оценку и обратную связь, связанную с этой отправкой, доступной студенту.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f43e158c5b6a59b45724aac5151e1f03d27a0c79
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860219"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="e6ab3-103">educationSubmission: Return</span><span class="sxs-lookup"><span data-stu-id="e6ab3-103">educationSubmission: return</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6ab3-104">Это действие делает оценку и обратную связь, связанную с этой отправкой, доступной студенту.</span><span class="sxs-lookup"><span data-stu-id="e6ab3-104">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="e6ab3-105">Это приведет к изменению состояния отправки с "Отправлено" на "возвращен" и указывает на то, что обратная связь передается или выполняется ступенчатое.</span><span class="sxs-lookup"><span data-stu-id="e6ab3-105">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="e6ab3-106">Это действие может выполнить только преподаватель.</span><span class="sxs-lookup"><span data-stu-id="e6ab3-106">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6ab3-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6ab3-107">Permissions</span></span>
<span data-ttu-id="e6ab3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6ab3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6ab3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6ab3-110">Permission type</span></span>      | <span data-ttu-id="e6ab3-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6ab3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6ab3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6ab3-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="e6ab3-113">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6ab3-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="e6ab3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6ab3-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e6ab3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6ab3-115">Not supported.</span></span>  |
|<span data-ttu-id="e6ab3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6ab3-116">Application</span></span> | <span data-ttu-id="e6ab3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6ab3-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e6ab3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6ab3-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="e6ab3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6ab3-119">Request headers</span></span>
| <span data-ttu-id="e6ab3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6ab3-120">Header</span></span>       | <span data-ttu-id="e6ab3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e6ab3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e6ab3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6ab3-122">Authorization</span></span>  | <span data-ttu-id="e6ab3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6ab3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e6ab3-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e6ab3-125">Request body</span></span>
<span data-ttu-id="e6ab3-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6ab3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6ab3-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6ab3-127">Response</span></span>
<span data-ttu-id="e6ab3-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e6ab3-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6ab3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e6ab3-130">Example</span></span>
<span data-ttu-id="e6ab3-131">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="e6ab3-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e6ab3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6ab3-132">Request</span></span>
<span data-ttu-id="e6ab3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6ab3-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e6ab3-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6ab3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e6ab3-135">C#</span><span class="sxs-lookup"><span data-stu-id="e6ab3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-return-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e6ab3-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="e6ab3-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-return-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e6ab3-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e6ab3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-return-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e6ab3-138">Java</span><span class="sxs-lookup"><span data-stu-id="e6ab3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-return-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e6ab3-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6ab3-139">Response</span></span>
<span data-ttu-id="e6ab3-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e6ab3-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
