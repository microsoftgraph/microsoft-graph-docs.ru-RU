---
title: 'educationSubmission: освобождение'
description: " и указывает, что выполняется оценка успеваемости. Это действие можно выполнить только с преподаватель."
ms.openlocfilehash: b521938737f9a3d8208c56ef5ee1b4091d075738
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077584"
---
# <a name="educationsubmission-release"></a><span data-ttu-id="a2832-104">educationSubmission: освобождение</span><span class="sxs-lookup"><span data-stu-id="a2832-104">educationSubmission: release</span></span>

> <span data-ttu-id="a2832-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a2832-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2832-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2832-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a2832-107">Это действие делает марки и отзыв, связанный с этой отправки доступные студента.</span><span class="sxs-lookup"><span data-stu-id="a2832-107">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="a2832-108">Это измените состояние подачи с «отправленные» на «выпущенная» и указывает, что выполняется оценка успеваемости.</span><span class="sxs-lookup"><span data-stu-id="a2832-108">This will change the status of the submission from "submitted" to "released" and indicates that grading is done.</span></span> <span data-ttu-id="a2832-109">Это действие можно выполнить только с преподаватель.</span><span class="sxs-lookup"><span data-stu-id="a2832-109">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="a2832-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2832-110">Permissions</span></span>
<span data-ttu-id="a2832-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2832-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2832-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2832-113">Permission type</span></span>      | <span data-ttu-id="a2832-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2832-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a2832-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2832-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="a2832-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a2832-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="a2832-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2832-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a2832-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2832-118">Not supported.</span></span>  |
|<span data-ttu-id="a2832-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2832-119">Application</span></span> | <span data-ttu-id="a2832-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2832-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a2832-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2832-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/release

```
## <a name="request-headers"></a><span data-ttu-id="a2832-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2832-122">Request headers</span></span>
| <span data-ttu-id="a2832-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2832-123">Header</span></span>       | <span data-ttu-id="a2832-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a2832-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a2832-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2832-125">Authorization</span></span>  | <span data-ttu-id="a2832-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2832-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a2832-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a2832-128">Request body</span></span>
<span data-ttu-id="a2832-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2832-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2832-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2832-130">Response</span></span>
<span data-ttu-id="a2832-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a2832-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2832-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a2832-133">Example</span></span>
<span data-ttu-id="a2832-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="a2832-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a2832-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2832-135">Request</span></span>
<span data-ttu-id="a2832-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a2832-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_release"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/release
```

##### <a name="response"></a><span data-ttu-id="a2832-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2832-137">Response</span></span>
<span data-ttu-id="a2832-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a2832-138">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: release",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->