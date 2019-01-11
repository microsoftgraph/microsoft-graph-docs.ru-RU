---
title: 'educationSubmission: освобождение'
description: " и указывает, что выполняется оценка успеваемости. Это действие можно выполнить только с преподаватель."
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: a2723684f734a9e31dc08fb97d1e184400cac387
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859012"
---
# <a name="educationsubmission-release"></a><span data-ttu-id="5ef66-104">educationSubmission: освобождение</span><span class="sxs-lookup"><span data-stu-id="5ef66-104">educationSubmission: release</span></span>

> <span data-ttu-id="5ef66-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5ef66-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ef66-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ef66-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5ef66-107">Это действие делает марки и отзыв, связанный с этой отправки доступные студента.</span><span class="sxs-lookup"><span data-stu-id="5ef66-107">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="5ef66-108">Это измените состояние подачи с «отправленные» на «выпущенная» и указывает, что выполняется оценка успеваемости.</span><span class="sxs-lookup"><span data-stu-id="5ef66-108">This will change the status of the submission from "submitted" to "released" and indicates that grading is done.</span></span> <span data-ttu-id="5ef66-109">Это действие можно выполнить только с преподаватель.</span><span class="sxs-lookup"><span data-stu-id="5ef66-109">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ef66-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ef66-110">Permissions</span></span>
<span data-ttu-id="5ef66-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ef66-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ef66-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ef66-113">Permission type</span></span>      | <span data-ttu-id="5ef66-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ef66-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ef66-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ef66-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="5ef66-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5ef66-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="5ef66-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ef66-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5ef66-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ef66-118">Not supported.</span></span>  |
|<span data-ttu-id="5ef66-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ef66-119">Application</span></span> | <span data-ttu-id="5ef66-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ef66-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5ef66-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ef66-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/release

```
## <a name="request-headers"></a><span data-ttu-id="5ef66-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ef66-122">Request headers</span></span>
| <span data-ttu-id="5ef66-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ef66-123">Header</span></span>       | <span data-ttu-id="5ef66-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5ef66-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5ef66-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ef66-125">Authorization</span></span>  | <span data-ttu-id="5ef66-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ef66-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ef66-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5ef66-128">Request body</span></span>
<span data-ttu-id="5ef66-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ef66-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ef66-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ef66-130">Response</span></span>
<span data-ttu-id="5ef66-p106">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5ef66-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ef66-133">Пример</span><span class="sxs-lookup"><span data-stu-id="5ef66-133">Example</span></span>
<span data-ttu-id="5ef66-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="5ef66-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5ef66-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ef66-135">Request</span></span>
<span data-ttu-id="5ef66-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5ef66-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_release"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/release
```

##### <a name="response"></a><span data-ttu-id="5ef66-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ef66-137">Response</span></span>
<span data-ttu-id="5ef66-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5ef66-138">The following is an example of the response.</span></span>

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
