---
title: 'educationSubmission: Return'
description: Это действие делает оценку и обратную связь, связанную с этой отправкой, доступной студенту.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 203fcc9efa06b9f34e5c1d9fbb0bc806cc1e6e10
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441403"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="87e9a-103">educationSubmission: Return</span><span class="sxs-lookup"><span data-stu-id="87e9a-103">educationSubmission: return</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87e9a-104">Это действие делает оценку и обратную связь, связанную с этой отправкой, доступной студенту.</span><span class="sxs-lookup"><span data-stu-id="87e9a-104">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="87e9a-105">Это приведет к изменению состояния отправки с "Отправлено" на "возвращен" и указывает на то, что обратная связь передается или выполняется ступенчатое.</span><span class="sxs-lookup"><span data-stu-id="87e9a-105">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="87e9a-106">Это действие может выполнить только преподаватель.</span><span class="sxs-lookup"><span data-stu-id="87e9a-106">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="87e9a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87e9a-107">Permissions</span></span>
<span data-ttu-id="87e9a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87e9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87e9a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87e9a-110">Permission type</span></span>      | <span data-ttu-id="87e9a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87e9a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87e9a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87e9a-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="87e9a-113">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87e9a-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="87e9a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87e9a-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="87e9a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87e9a-115">Not supported.</span></span>  |
|<span data-ttu-id="87e9a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87e9a-116">Application</span></span> | <span data-ttu-id="87e9a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87e9a-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="87e9a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87e9a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="87e9a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87e9a-119">Request headers</span></span>
| <span data-ttu-id="87e9a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87e9a-120">Header</span></span>       | <span data-ttu-id="87e9a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="87e9a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="87e9a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87e9a-122">Authorization</span></span>  | <span data-ttu-id="87e9a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87e9a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="87e9a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="87e9a-125">Request body</span></span>
<span data-ttu-id="87e9a-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="87e9a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87e9a-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="87e9a-127">Response</span></span>
<span data-ttu-id="87e9a-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="87e9a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87e9a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="87e9a-130">Example</span></span>
<span data-ttu-id="87e9a-131">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="87e9a-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="87e9a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="87e9a-132">Request</span></span>
<span data-ttu-id="87e9a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87e9a-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="87e9a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="87e9a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="87e9a-135">C#</span><span class="sxs-lookup"><span data-stu-id="87e9a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-return-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="87e9a-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="87e9a-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-return-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="87e9a-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="87e9a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-return-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="87e9a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="87e9a-138">Response</span></span>
<span data-ttu-id="87e9a-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="87e9a-139">The following is an example of the response.</span></span>

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
