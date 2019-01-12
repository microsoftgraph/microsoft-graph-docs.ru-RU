---
title: 'educationSubmission: unsubmit'
description: 'Действие, которое указывает, что студента работает на отправки назначения после включения. Это действие может быть занято только учащегося. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: fc17216800c39f0a094ba5f8d9f281394ba7e2de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945470"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="991f0-104">educationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="991f0-104">educationSubmission: unsubmit</span></span>

> <span data-ttu-id="991f0-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="991f0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="991f0-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="991f0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="991f0-107">Действие, которое указывает, что студента работает на отправки назначения после включения.</span><span class="sxs-lookup"><span data-stu-id="991f0-107">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="991f0-108">Это действие может быть занято только учащегося.</span><span class="sxs-lookup"><span data-stu-id="991f0-108">This action can only be taken by the student.</span></span> <span data-ttu-id="991f0-109">Состояние отправки из «отправленные» изменится на «работа».</span><span class="sxs-lookup"><span data-stu-id="991f0-109">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="991f0-110">Во время процесса отправки все ресурсы копируются из submittedResources интервалов workingResources.</span><span class="sxs-lookup"><span data-stu-id="991f0-110">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="991f0-111">Преподаватель выполнит поиск в списке ресурсы рабочее для ранжирования.</span><span class="sxs-lookup"><span data-stu-id="991f0-111">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="991f0-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="991f0-112">Permissions</span></span>
<span data-ttu-id="991f0-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="991f0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="991f0-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="991f0-115">Permission type</span></span>      | <span data-ttu-id="991f0-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="991f0-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="991f0-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="991f0-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="991f0-118">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="991f0-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="991f0-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="991f0-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="991f0-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="991f0-120">Not supported.</span></span>  |
|<span data-ttu-id="991f0-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="991f0-121">Application</span></span> | <span data-ttu-id="991f0-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="991f0-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="991f0-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="991f0-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="991f0-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="991f0-124">Request headers</span></span>
| <span data-ttu-id="991f0-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="991f0-125">Header</span></span>       | <span data-ttu-id="991f0-126">Значение</span><span class="sxs-lookup"><span data-stu-id="991f0-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="991f0-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="991f0-127">Authorization</span></span>  | <span data-ttu-id="991f0-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="991f0-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="991f0-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="991f0-130">Request body</span></span>
<span data-ttu-id="991f0-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="991f0-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="991f0-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="991f0-132">Response</span></span>
<span data-ttu-id="991f0-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="991f0-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="991f0-135">Пример</span><span class="sxs-lookup"><span data-stu-id="991f0-135">Example</span></span>
<span data-ttu-id="991f0-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="991f0-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="991f0-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="991f0-137">Request</span></span>
<span data-ttu-id="991f0-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="991f0-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```

##### <a name="response"></a><span data-ttu-id="991f0-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="991f0-139">Response</span></span>
<span data-ttu-id="991f0-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="991f0-140">The following is an example of the response.</span></span>

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
