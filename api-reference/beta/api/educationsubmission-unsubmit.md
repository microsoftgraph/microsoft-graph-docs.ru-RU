---
title: 'educationSubmission: unsubmit'
description: 'Действие, которое указывает, что студента работает на отправки назначения после включения. Это действие может быть занято только учащегося. '
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 853dce22c7c79ffda7b823794259fa7be0363d02
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829220"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="c9822-104">educationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="c9822-104">educationSubmission: unsubmit</span></span>

> <span data-ttu-id="c9822-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c9822-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9822-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9822-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9822-107">Действие, которое указывает, что студента работает на отправки назначения после включения.</span><span class="sxs-lookup"><span data-stu-id="c9822-107">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="c9822-108">Это действие может быть занято только учащегося.</span><span class="sxs-lookup"><span data-stu-id="c9822-108">This action can only be taken by the student.</span></span> <span data-ttu-id="c9822-109">Состояние отправки из «отправленные» изменится на «работа».</span><span class="sxs-lookup"><span data-stu-id="c9822-109">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="c9822-110">Во время процесса отправки все ресурсы копируются из submittedResources интервалов workingResources.</span><span class="sxs-lookup"><span data-stu-id="c9822-110">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="c9822-111">Преподаватель выполнит поиск в списке ресурсы рабочее для ранжирования.</span><span class="sxs-lookup"><span data-stu-id="c9822-111">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9822-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9822-112">Permissions</span></span>
<span data-ttu-id="c9822-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9822-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9822-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9822-115">Permission type</span></span>      | <span data-ttu-id="c9822-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9822-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9822-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9822-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="c9822-118">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9822-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="c9822-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9822-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c9822-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9822-120">Not supported.</span></span>  |
|<span data-ttu-id="c9822-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9822-121">Application</span></span> | <span data-ttu-id="c9822-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9822-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c9822-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9822-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="c9822-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9822-124">Request headers</span></span>
| <span data-ttu-id="c9822-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9822-125">Header</span></span>       | <span data-ttu-id="c9822-126">Значение</span><span class="sxs-lookup"><span data-stu-id="c9822-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c9822-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9822-127">Authorization</span></span>  | <span data-ttu-id="c9822-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9822-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c9822-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9822-130">Request body</span></span>
<span data-ttu-id="c9822-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9822-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9822-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9822-132">Response</span></span>
<span data-ttu-id="c9822-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c9822-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9822-135">Пример</span><span class="sxs-lookup"><span data-stu-id="c9822-135">Example</span></span>
<span data-ttu-id="c9822-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="c9822-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c9822-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9822-137">Request</span></span>
<span data-ttu-id="c9822-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9822-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```

##### <a name="response"></a><span data-ttu-id="c9822-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9822-139">Response</span></span>
<span data-ttu-id="c9822-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c9822-140">The following is an example of the response.</span></span>

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
