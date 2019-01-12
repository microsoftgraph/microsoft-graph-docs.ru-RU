---
title: 'educationSubmission: возврата'
description: Это действие делает марки и отзыв, связанный с этой отправки доступные студента.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 39e57044571b43df0515755035e23a38980376fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930651"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="6b23a-103">educationSubmission: возврата</span><span class="sxs-lookup"><span data-stu-id="6b23a-103">educationSubmission: return</span></span>

> <span data-ttu-id="6b23a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6b23a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b23a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b23a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b23a-106">Это действие делает марки и отзыв, связанный с этой отправки доступные студента.</span><span class="sxs-lookup"><span data-stu-id="6b23a-106">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="6b23a-107">Это изменение состояния подачи из «отправленные» «вернуть» и указывает на то, что обратной связи или оценка успеваемости выполняется.</span><span class="sxs-lookup"><span data-stu-id="6b23a-107">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="6b23a-108">Это действие можно выполнить только с преподаватель.</span><span class="sxs-lookup"><span data-stu-id="6b23a-108">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b23a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b23a-109">Permissions</span></span>
<span data-ttu-id="6b23a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b23a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b23a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b23a-112">Permission type</span></span>      | <span data-ttu-id="6b23a-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b23a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b23a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b23a-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="6b23a-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6b23a-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="6b23a-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b23a-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6b23a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b23a-117">Not supported.</span></span>  |
|<span data-ttu-id="6b23a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b23a-118">Application</span></span> | <span data-ttu-id="6b23a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b23a-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6b23a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b23a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="6b23a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b23a-121">Request headers</span></span>
| <span data-ttu-id="6b23a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b23a-122">Header</span></span>       | <span data-ttu-id="6b23a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="6b23a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6b23a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b23a-124">Authorization</span></span>  | <span data-ttu-id="6b23a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b23a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6b23a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6b23a-127">Request body</span></span>
<span data-ttu-id="6b23a-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6b23a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b23a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b23a-129">Response</span></span>
<span data-ttu-id="6b23a-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6b23a-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b23a-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6b23a-132">Example</span></span>
<span data-ttu-id="6b23a-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="6b23a-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6b23a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b23a-134">Request</span></span>
<span data-ttu-id="6b23a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b23a-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="6b23a-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b23a-136">Response</span></span>
<span data-ttu-id="6b23a-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6b23a-137">The following is an example of the response.</span></span>

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
