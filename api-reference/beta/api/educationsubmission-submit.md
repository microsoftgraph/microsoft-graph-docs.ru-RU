---
title: 'educationSubmission: Отправка'
description: . Во время процесса отправки интервалов submittedResources будут скопированы все ресурсы. Преподаватель выполнит поиск в списке добавленных ресурсы для ранжирования.
ms.openlocfilehash: 566948278ffacb1169842c49aa11c78cba0a5f3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076568"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="d779b-105">educationSubmission: Отправка</span><span class="sxs-lookup"><span data-stu-id="d779b-105">educationSubmission: submit</span></span>

> <span data-ttu-id="d779b-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d779b-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d779b-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d779b-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d779b-108">Действие, которое указывает, что студента выполняется с работой и готов к передаче в назначении.</span><span class="sxs-lookup"><span data-stu-id="d779b-108">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="d779b-109">Это действие может быть занято только учащегося.</span><span class="sxs-lookup"><span data-stu-id="d779b-109">This action can only be taken by the student.</span></span> <span data-ttu-id="d779b-110">Это будет изменено состояние отправки из «рабочий» на «отправленные».</span><span class="sxs-lookup"><span data-stu-id="d779b-110">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="d779b-111">Во время процесса отправки интервалов submittedResources будут скопированы все ресурсы.</span><span class="sxs-lookup"><span data-stu-id="d779b-111">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="d779b-112">Преподаватель выполнит поиск в списке добавленных ресурсы для ранжирования.</span><span class="sxs-lookup"><span data-stu-id="d779b-112">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="d779b-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d779b-113">Permissions</span></span>
<span data-ttu-id="d779b-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d779b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d779b-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d779b-116">Permission type</span></span>      | <span data-ttu-id="d779b-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d779b-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d779b-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d779b-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="d779b-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d779b-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d779b-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d779b-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d779b-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d779b-121">Not supported.</span></span>  |
|<span data-ttu-id="d779b-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d779b-122">Application</span></span> | <span data-ttu-id="d779b-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d779b-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d779b-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d779b-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="d779b-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d779b-125">Request headers</span></span>
| <span data-ttu-id="d779b-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d779b-126">Header</span></span>       | <span data-ttu-id="d779b-127">Значение</span><span class="sxs-lookup"><span data-stu-id="d779b-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d779b-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d779b-128">Authorization</span></span>  | <span data-ttu-id="d779b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d779b-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d779b-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d779b-131">Request body</span></span>
<span data-ttu-id="d779b-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d779b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d779b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d779b-133">Response</span></span>
<span data-ttu-id="d779b-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d779b-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d779b-136">Пример</span><span class="sxs-lookup"><span data-stu-id="d779b-136">Example</span></span>
<span data-ttu-id="d779b-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="d779b-137">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d779b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="d779b-138">Request</span></span>
<span data-ttu-id="d779b-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d779b-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="d779b-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="d779b-140">Response</span></span>
<span data-ttu-id="d779b-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d779b-141">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->