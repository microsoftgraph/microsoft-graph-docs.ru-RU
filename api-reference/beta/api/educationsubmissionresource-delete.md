---
title: Удаление educationSubmissionResource
description: " ресурсов в исходное состояние. Если ресурс не был скопирован из назначения, но был добавлен из студента, ресурса просто удален."
ms.openlocfilehash: 9eb5b08e2e5481e707cc6c1e0b0f8339e3d22ad4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079765"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="9c736-104">Удаление educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="9c736-104">Delete educationSubmissionResource</span></span>

> <span data-ttu-id="9c736-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9c736-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c736-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c736-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9c736-107">Удаляет ресурс из подачи.</span><span class="sxs-lookup"><span data-stu-id="9c736-107">Deletes a resource from the submission.</span></span> <span data-ttu-id="9c736-108">Это может быть выполнено только с учащегося.</span><span class="sxs-lookup"><span data-stu-id="9c736-108">This can only be done by the student.</span></span> <span data-ttu-id="9c736-109">Если ресурс был скопирован из назначения, новую копию ресурса создается после удаления текущей копии.</span><span class="sxs-lookup"><span data-stu-id="9c736-109">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="9c736-110">Это позволяет «Сброс» ресурса в исходное состояние.</span><span class="sxs-lookup"><span data-stu-id="9c736-110">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="9c736-111">Если ресурс не был скопирован из назначения, но был добавлен из студента, ресурса просто удален.</span><span class="sxs-lookup"><span data-stu-id="9c736-111">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c736-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c736-112">Permissions</span></span>
<span data-ttu-id="9c736-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c736-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c736-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c736-115">Permission type</span></span>      | <span data-ttu-id="9c736-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c736-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c736-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c736-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="9c736-118">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c736-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="9c736-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c736-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9c736-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c736-120">Not supported.</span></span>  |
|<span data-ttu-id="9c736-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c736-121">Application</span></span> | <span data-ttu-id="9c736-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c736-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9c736-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c736-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9c736-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c736-124">Request headers</span></span>
| <span data-ttu-id="9c736-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c736-125">Header</span></span>       | <span data-ttu-id="9c736-126">Значение</span><span class="sxs-lookup"><span data-stu-id="9c736-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9c736-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c736-127">Authorization</span></span>  | <span data-ttu-id="9c736-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c736-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9c736-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c736-130">Request body</span></span>
<span data-ttu-id="9c736-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c736-131">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9c736-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c736-132">Response</span></span>
<span data-ttu-id="9c736-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9c736-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c736-135">Пример</span><span class="sxs-lookup"><span data-stu-id="9c736-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c736-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c736-136">Request</span></span>
<span data-ttu-id="9c736-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c736-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="9c736-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c736-138">Response</span></span>
<span data-ttu-id="9c736-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9c736-139">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->