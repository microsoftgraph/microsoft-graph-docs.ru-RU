---
title: 'educationSubmission: отзыв'
description: .
ms.openlocfilehash: 8df134a6d8325e5b497baada89bc0fa16d0ee9e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075661"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="246db-103">educationSubmission: отзыв</span><span class="sxs-lookup"><span data-stu-id="246db-103">educationSubmission: recall</span></span>

> <span data-ttu-id="246db-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="246db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="246db-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="246db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="246db-106">Указывает, что студента хочет вернуть отправку.</span><span class="sxs-lookup"><span data-stu-id="246db-106">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="246db-107">Это действие можно выполнить только с студента.</span><span class="sxs-lookup"><span data-stu-id="246db-107">This action can only be done by a student.</span></span> <span data-ttu-id="246db-108">Оно будет изменен состояние подачи «отправленные» вернуться к «рабочий».</span><span class="sxs-lookup"><span data-stu-id="246db-108">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="246db-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="246db-109">Permissions</span></span>
<span data-ttu-id="246db-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="246db-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="246db-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="246db-112">Permission type</span></span>      | <span data-ttu-id="246db-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="246db-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="246db-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="246db-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="246db-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="246db-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="246db-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="246db-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="246db-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="246db-117">Not supported</span></span>  |
|<span data-ttu-id="246db-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="246db-118">Application</span></span> |<span data-ttu-id="246db-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="246db-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="246db-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="246db-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="246db-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="246db-121">Request headers</span></span>
| <span data-ttu-id="246db-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="246db-122">Header</span></span>       | <span data-ttu-id="246db-123">Значение</span><span class="sxs-lookup"><span data-stu-id="246db-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="246db-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="246db-124">Authorization</span></span>  | <span data-ttu-id="246db-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="246db-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="246db-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="246db-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="246db-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="246db-128">Response</span></span>
<span data-ttu-id="246db-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="246db-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="246db-131">Пример</span><span class="sxs-lookup"><span data-stu-id="246db-131">Example</span></span>
<span data-ttu-id="246db-132">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="246db-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="246db-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="246db-133">Request</span></span>
<span data-ttu-id="246db-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="246db-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="246db-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="246db-135">Response</span></span>
<span data-ttu-id="246db-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="246db-136">The following is an example of the response.</span></span>

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