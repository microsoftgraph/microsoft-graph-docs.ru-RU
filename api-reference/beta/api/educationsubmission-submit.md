---
title: 'educationSubmission: Отправка'
description: Действие, которое указывает, что студента выполняется с работой и готов к передаче в назначении. Это действие может быть занято только учащегося.
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: ef2ef84819a6bfbeeb83a012b4c26fe7cb56662c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808577"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="99885-104">educationSubmission: Отправка</span><span class="sxs-lookup"><span data-stu-id="99885-104">educationSubmission: submit</span></span>

> <span data-ttu-id="99885-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="99885-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99885-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99885-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99885-107">Действие, которое указывает, что студента выполняется с работой и готов к передаче в назначении.</span><span class="sxs-lookup"><span data-stu-id="99885-107">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="99885-108">Это действие может быть занято только учащегося.</span><span class="sxs-lookup"><span data-stu-id="99885-108">This action can only be taken by the student.</span></span> <span data-ttu-id="99885-109">Это будет изменено состояние отправки из «рабочий» на «отправленные».</span><span class="sxs-lookup"><span data-stu-id="99885-109">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="99885-110">Во время процесса отправки интервалов submittedResources будут скопированы все ресурсы.</span><span class="sxs-lookup"><span data-stu-id="99885-110">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="99885-111">Преподаватель выполнит поиск в списке добавленных ресурсы для ранжирования.</span><span class="sxs-lookup"><span data-stu-id="99885-111">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="99885-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99885-112">Permissions</span></span>
<span data-ttu-id="99885-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99885-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99885-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99885-115">Permission type</span></span>      | <span data-ttu-id="99885-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99885-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99885-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99885-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="99885-118">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="99885-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="99885-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99885-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="99885-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99885-120">Not supported.</span></span>  |
|<span data-ttu-id="99885-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99885-121">Application</span></span> | <span data-ttu-id="99885-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99885-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="99885-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99885-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="99885-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99885-124">Request headers</span></span>
| <span data-ttu-id="99885-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99885-125">Header</span></span>       | <span data-ttu-id="99885-126">Значение</span><span class="sxs-lookup"><span data-stu-id="99885-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="99885-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99885-127">Authorization</span></span>  | <span data-ttu-id="99885-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99885-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="99885-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="99885-130">Request body</span></span>
<span data-ttu-id="99885-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="99885-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99885-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="99885-132">Response</span></span>
<span data-ttu-id="99885-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="99885-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99885-135">Пример</span><span class="sxs-lookup"><span data-stu-id="99885-135">Example</span></span>
<span data-ttu-id="99885-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="99885-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="99885-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="99885-137">Request</span></span>
<span data-ttu-id="99885-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99885-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```

##### <a name="response"></a><span data-ttu-id="99885-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="99885-139">Response</span></span>
<span data-ttu-id="99885-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="99885-140">The following is an example of the response.</span></span>

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
