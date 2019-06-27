---
title: 'educationSubmission: Return'
description: Это действие делает оценку и обратную связь, связанную с этой отправкой, доступной студенту.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 60d470dbfe80620e477a2b60cd47a875ca7ad043
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259495"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="0c5e4-103">educationSubmission: Return</span><span class="sxs-lookup"><span data-stu-id="0c5e4-103">educationSubmission: return</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c5e4-104">Это действие делает оценку и обратную связь, связанную с этой отправкой, доступной студенту.</span><span class="sxs-lookup"><span data-stu-id="0c5e4-104">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="0c5e4-105">Это приведет к изменению состояния отправки с "Отправлено" на "возвращен" и указывает на то, что обратная связь передается или выполняется ступенчатое.</span><span class="sxs-lookup"><span data-stu-id="0c5e4-105">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="0c5e4-106">Это действие может выполнить только преподаватель.</span><span class="sxs-lookup"><span data-stu-id="0c5e4-106">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c5e4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0c5e4-107">Permissions</span></span>
<span data-ttu-id="0c5e4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c5e4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c5e4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c5e4-110">Permission type</span></span>      | <span data-ttu-id="0c5e4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c5e4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c5e4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c5e4-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="0c5e4-113">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0c5e4-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="0c5e4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c5e4-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0c5e4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c5e4-115">Not supported.</span></span>  |
|<span data-ttu-id="0c5e4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c5e4-116">Application</span></span> | <span data-ttu-id="0c5e4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c5e4-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0c5e4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c5e4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="0c5e4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c5e4-119">Request headers</span></span>
| <span data-ttu-id="0c5e4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c5e4-120">Header</span></span>       | <span data-ttu-id="0c5e4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0c5e4-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0c5e4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0c5e4-122">Authorization</span></span>  | <span data-ttu-id="0c5e4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c5e4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0c5e4-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0c5e4-125">Request body</span></span>
<span data-ttu-id="0c5e4-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0c5e4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c5e4-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c5e4-127">Response</span></span>
<span data-ttu-id="0c5e4-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0c5e4-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c5e4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="0c5e4-130">Example</span></span>
<span data-ttu-id="0c5e4-131">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="0c5e4-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0c5e4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c5e4-132">Request</span></span>
<span data-ttu-id="0c5e4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c5e4-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="0c5e4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c5e4-134">Response</span></span>
<span data-ttu-id="0c5e4-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0c5e4-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0c5e4-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="0c5e4-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0c5e4-137">C#</span><span class="sxs-lookup"><span data-stu-id="0c5e4-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/educationsubmission_return-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c5e4-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="0c5e4-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/educationsubmission_return-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0c5e4-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0c5e4-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/educationsubmission_return-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/educationsubmission-return.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationsubmission-return.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsubmission-return.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
