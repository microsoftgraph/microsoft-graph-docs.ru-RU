---
title: 'educationSubmission: отзыв'
description: 'Указывает, что студента хочет вернуть отправку. Это действие можно выполнить только с студента. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9e9155244522d7f1f8c61263aff6de4c87faab4e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984411"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="23ca2-104">educationSubmission: отзыв</span><span class="sxs-lookup"><span data-stu-id="23ca2-104">educationSubmission: recall</span></span>

> <span data-ttu-id="23ca2-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="23ca2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23ca2-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23ca2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23ca2-107">Указывает, что студента хочет вернуть отправку.</span><span class="sxs-lookup"><span data-stu-id="23ca2-107">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="23ca2-108">Это действие можно выполнить только с студента.</span><span class="sxs-lookup"><span data-stu-id="23ca2-108">This action can only be done by a student.</span></span> <span data-ttu-id="23ca2-109">Оно будет изменен состояние подачи «отправленные» вернуться к «рабочий».</span><span class="sxs-lookup"><span data-stu-id="23ca2-109">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="23ca2-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23ca2-110">Permissions</span></span>
<span data-ttu-id="23ca2-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23ca2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23ca2-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23ca2-113">Permission type</span></span>      | <span data-ttu-id="23ca2-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23ca2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23ca2-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23ca2-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="23ca2-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23ca2-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="23ca2-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23ca2-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="23ca2-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="23ca2-118">Not supported</span></span>  |
|<span data-ttu-id="23ca2-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23ca2-119">Application</span></span> |<span data-ttu-id="23ca2-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23ca2-120">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="23ca2-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23ca2-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="23ca2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23ca2-122">Request headers</span></span>
| <span data-ttu-id="23ca2-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23ca2-123">Header</span></span>       | <span data-ttu-id="23ca2-124">Значение</span><span class="sxs-lookup"><span data-stu-id="23ca2-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="23ca2-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23ca2-125">Authorization</span></span>  | <span data-ttu-id="23ca2-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23ca2-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="23ca2-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="23ca2-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="23ca2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="23ca2-129">Response</span></span>
<span data-ttu-id="23ca2-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="23ca2-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23ca2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="23ca2-132">Example</span></span>
<span data-ttu-id="23ca2-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="23ca2-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="23ca2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="23ca2-134">Request</span></span>
<span data-ttu-id="23ca2-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23ca2-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="23ca2-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="23ca2-136">Response</span></span>
<span data-ttu-id="23ca2-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="23ca2-137">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: recall",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
