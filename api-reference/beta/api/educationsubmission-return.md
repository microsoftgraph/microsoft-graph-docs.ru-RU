---
title: 'educationSubmission: Return'
description: Это действие делает оценку и обратную связь, связанную с этой отправкой, доступной студенту.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d04c954f239ba1999f2ca838d14e52b7920f4bc0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424829"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="13808-103">educationSubmission: Return</span><span class="sxs-lookup"><span data-stu-id="13808-103">educationSubmission: return</span></span>

<span data-ttu-id="13808-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="13808-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13808-105">Это действие делает оценку и обратную связь, связанную с этой отправкой, доступной студенту.</span><span class="sxs-lookup"><span data-stu-id="13808-105">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="13808-106">Это приведет к изменению состояния отправки с "Отправлено" на "возвращен" и указывает на то, что обратная связь передается или выполняется ступенчатое.</span><span class="sxs-lookup"><span data-stu-id="13808-106">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="13808-107">Это действие может выполнить только преподаватель.</span><span class="sxs-lookup"><span data-stu-id="13808-107">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="13808-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="13808-108">Permissions</span></span>
<span data-ttu-id="13808-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13808-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13808-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="13808-111">Permission type</span></span>      | <span data-ttu-id="13808-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="13808-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13808-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="13808-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="13808-114">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="13808-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="13808-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="13808-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="13808-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13808-116">Not supported.</span></span>  |
|<span data-ttu-id="13808-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="13808-117">Application</span></span> | <span data-ttu-id="13808-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13808-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="13808-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="13808-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="13808-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="13808-120">Request headers</span></span>
| <span data-ttu-id="13808-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="13808-121">Header</span></span>       | <span data-ttu-id="13808-122">Значение</span><span class="sxs-lookup"><span data-stu-id="13808-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="13808-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="13808-123">Authorization</span></span>  | <span data-ttu-id="13808-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="13808-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="13808-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="13808-126">Request body</span></span>
<span data-ttu-id="13808-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="13808-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13808-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="13808-128">Response</span></span>
<span data-ttu-id="13808-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="13808-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13808-131">Пример</span><span class="sxs-lookup"><span data-stu-id="13808-131">Example</span></span>
<span data-ttu-id="13808-132">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="13808-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="13808-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="13808-133">Request</span></span>
<span data-ttu-id="13808-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="13808-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="13808-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="13808-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```
# <a name="c"></a>[<span data-ttu-id="13808-136">C#</span><span class="sxs-lookup"><span data-stu-id="13808-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-return-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13808-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13808-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-return-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13808-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13808-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-return-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="13808-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="13808-139">Response</span></span>
<span data-ttu-id="13808-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="13808-140">The following is an example of the response.</span></span>

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
