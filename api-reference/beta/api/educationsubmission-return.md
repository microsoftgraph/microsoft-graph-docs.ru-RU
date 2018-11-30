---
title: 'educationSubmission: возврата'
description: " и указывает на то, что обратной связи или оценка успеваемости выполняется. Это действие можно выполнить только с преподаватель."
ms.openlocfilehash: de81f5429119556753462781f701fb7c936826b1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074707"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="177bd-104">educationSubmission: возврата</span><span class="sxs-lookup"><span data-stu-id="177bd-104">educationSubmission: return</span></span>

> <span data-ttu-id="177bd-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="177bd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="177bd-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="177bd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="177bd-107">Это действие делает марки и отзыв, связанный с этой отправки доступные студента.</span><span class="sxs-lookup"><span data-stu-id="177bd-107">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="177bd-108">Это изменение состояния подачи из «отправленные» «вернуть» и указывает на то, что обратной связи или оценка успеваемости выполняется.</span><span class="sxs-lookup"><span data-stu-id="177bd-108">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="177bd-109">Это действие можно выполнить только с преподаватель.</span><span class="sxs-lookup"><span data-stu-id="177bd-109">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="177bd-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="177bd-110">Permissions</span></span>
<span data-ttu-id="177bd-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="177bd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="177bd-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="177bd-113">Permission type</span></span>      | <span data-ttu-id="177bd-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="177bd-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="177bd-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="177bd-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="177bd-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="177bd-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="177bd-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="177bd-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="177bd-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="177bd-118">Not supported.</span></span>  |
|<span data-ttu-id="177bd-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="177bd-119">Application</span></span> | <span data-ttu-id="177bd-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="177bd-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="177bd-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="177bd-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="177bd-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="177bd-122">Request headers</span></span>
| <span data-ttu-id="177bd-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="177bd-123">Header</span></span>       | <span data-ttu-id="177bd-124">Значение</span><span class="sxs-lookup"><span data-stu-id="177bd-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="177bd-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="177bd-125">Authorization</span></span>  | <span data-ttu-id="177bd-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="177bd-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="177bd-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="177bd-128">Request body</span></span>
<span data-ttu-id="177bd-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="177bd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="177bd-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="177bd-130">Response</span></span>
<span data-ttu-id="177bd-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="177bd-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="177bd-133">Пример</span><span class="sxs-lookup"><span data-stu-id="177bd-133">Example</span></span>
<span data-ttu-id="177bd-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="177bd-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="177bd-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="177bd-135">Request</span></span>
<span data-ttu-id="177bd-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="177bd-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="177bd-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="177bd-137">Response</span></span>
<span data-ttu-id="177bd-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="177bd-138">The following is an example of the response.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->