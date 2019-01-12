---
title: 'educationSubmission: Отправка'
description: Действие, которое указывает, что студента выполняется с работой и готов к передаче в назначении. Это действие может быть занято только учащегося.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d1fd41c66e3f54898f6086a9bf14a0b53763df88
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915811"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="b7c2e-104">educationSubmission: Отправка</span><span class="sxs-lookup"><span data-stu-id="b7c2e-104">educationSubmission: submit</span></span>

> <span data-ttu-id="b7c2e-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b7c2e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7c2e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7c2e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7c2e-107">Действие, которое указывает, что студента выполняется с работой и готов к передаче в назначении.</span><span class="sxs-lookup"><span data-stu-id="b7c2e-107">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="b7c2e-108">Это действие может быть занято только учащегося.</span><span class="sxs-lookup"><span data-stu-id="b7c2e-108">This action can only be taken by the student.</span></span> <span data-ttu-id="b7c2e-109">Это будет изменено состояние отправки из «рабочий» на «отправленные».</span><span class="sxs-lookup"><span data-stu-id="b7c2e-109">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="b7c2e-110">Во время процесса отправки интервалов submittedResources будут скопированы все ресурсы.</span><span class="sxs-lookup"><span data-stu-id="b7c2e-110">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="b7c2e-111">Преподаватель выполнит поиск в списке добавленных ресурсы для ранжирования.</span><span class="sxs-lookup"><span data-stu-id="b7c2e-111">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7c2e-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7c2e-112">Permissions</span></span>
<span data-ttu-id="b7c2e-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7c2e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7c2e-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7c2e-115">Permission type</span></span>      | <span data-ttu-id="b7c2e-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7c2e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7c2e-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7c2e-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="b7c2e-118">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b7c2e-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="b7c2e-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7c2e-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b7c2e-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7c2e-120">Not supported.</span></span>  |
|<span data-ttu-id="b7c2e-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7c2e-121">Application</span></span> | <span data-ttu-id="b7c2e-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7c2e-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b7c2e-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7c2e-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="b7c2e-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7c2e-124">Request headers</span></span>
| <span data-ttu-id="b7c2e-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7c2e-125">Header</span></span>       | <span data-ttu-id="b7c2e-126">Значение</span><span class="sxs-lookup"><span data-stu-id="b7c2e-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b7c2e-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7c2e-127">Authorization</span></span>  | <span data-ttu-id="b7c2e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7c2e-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b7c2e-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b7c2e-130">Request body</span></span>
<span data-ttu-id="b7c2e-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7c2e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7c2e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7c2e-132">Response</span></span>
<span data-ttu-id="b7c2e-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b7c2e-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7c2e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="b7c2e-135">Example</span></span>
<span data-ttu-id="b7c2e-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b7c2e-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b7c2e-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7c2e-137">Request</span></span>
<span data-ttu-id="b7c2e-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7c2e-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="b7c2e-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7c2e-139">Response</span></span>
<span data-ttu-id="b7c2e-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b7c2e-140">The following is an example of the response.</span></span>

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
