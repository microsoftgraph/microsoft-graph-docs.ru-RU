---
title: 'educationSubmission: unsubmit'
description: . Во время процесса отправки все ресурсы копируются из submittedResources интервалов workingResources. Преподаватель выполнит поиск в списке ресурсы рабочее для ранжирования.
ms.openlocfilehash: 610b5a69a06c29d2e2b9b1fa6eb501a56d59b076
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075671"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="9b378-105">educationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="9b378-105">educationSubmission: unsubmit</span></span>

> <span data-ttu-id="9b378-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9b378-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b378-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b378-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9b378-108">Действие, которое указывает, что студента работает на отправки назначения после включения.</span><span class="sxs-lookup"><span data-stu-id="9b378-108">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="9b378-109">Это действие может быть занято только учащегося.</span><span class="sxs-lookup"><span data-stu-id="9b378-109">This action can only be taken by the student.</span></span> <span data-ttu-id="9b378-110">Состояние отправки из «отправленные» изменится на «работа».</span><span class="sxs-lookup"><span data-stu-id="9b378-110">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="9b378-111">Во время процесса отправки все ресурсы копируются из submittedResources интервалов workingResources.</span><span class="sxs-lookup"><span data-stu-id="9b378-111">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="9b378-112">Преподаватель выполнит поиск в списке ресурсы рабочее для ранжирования.</span><span class="sxs-lookup"><span data-stu-id="9b378-112">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b378-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b378-113">Permissions</span></span>
<span data-ttu-id="9b378-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b378-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b378-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b378-116">Permission type</span></span>      | <span data-ttu-id="9b378-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b378-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b378-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b378-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="9b378-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9b378-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="9b378-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b378-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9b378-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b378-121">Not supported.</span></span>  |
|<span data-ttu-id="9b378-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b378-122">Application</span></span> | <span data-ttu-id="9b378-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b378-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9b378-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b378-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="9b378-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b378-125">Request headers</span></span>
| <span data-ttu-id="9b378-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b378-126">Header</span></span>       | <span data-ttu-id="9b378-127">Значение</span><span class="sxs-lookup"><span data-stu-id="9b378-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9b378-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b378-128">Authorization</span></span>  | <span data-ttu-id="9b378-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b378-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9b378-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b378-131">Request body</span></span>
<span data-ttu-id="9b378-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9b378-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b378-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b378-133">Response</span></span>
<span data-ttu-id="9b378-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9b378-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b378-136">Пример</span><span class="sxs-lookup"><span data-stu-id="9b378-136">Example</span></span>
<span data-ttu-id="9b378-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="9b378-137">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9b378-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b378-138">Request</span></span>
<span data-ttu-id="9b378-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b378-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```

##### <a name="response"></a><span data-ttu-id="9b378-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="9b378-140">Response</span></span>
<span data-ttu-id="9b378-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9b378-141">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: unsubmit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
