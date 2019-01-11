---
title: Удаление educationSubmissionResource
description: Удаляет ресурс из подачи. Это может быть выполнено только с учащегося. Если ресурс был скопирован из назначения, новую копию ресурса создается после удаления текущей копии.
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 94e73f7b4c6c0c0bc85b21ee3e651f8e61234e80
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828814"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="d2497-105">Удаление educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="d2497-105">Delete educationSubmissionResource</span></span>

> <span data-ttu-id="d2497-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d2497-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2497-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2497-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2497-108">Удаляет ресурс из подачи.</span><span class="sxs-lookup"><span data-stu-id="d2497-108">Deletes a resource from the submission.</span></span> <span data-ttu-id="d2497-109">Это может быть выполнено только с учащегося.</span><span class="sxs-lookup"><span data-stu-id="d2497-109">This can only be done by the student.</span></span> <span data-ttu-id="d2497-110">Если ресурс был скопирован из назначения, новую копию ресурса создается после удаления текущей копии.</span><span class="sxs-lookup"><span data-stu-id="d2497-110">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="d2497-111">Это позволяет «Сброс» ресурса в исходное состояние.</span><span class="sxs-lookup"><span data-stu-id="d2497-111">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="d2497-112">Если ресурс не был скопирован из назначения, но был добавлен из студента, ресурса просто удален.</span><span class="sxs-lookup"><span data-stu-id="d2497-112">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2497-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2497-113">Permissions</span></span>
<span data-ttu-id="d2497-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2497-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2497-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2497-116">Permission type</span></span>      | <span data-ttu-id="d2497-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2497-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2497-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2497-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="d2497-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2497-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d2497-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2497-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d2497-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2497-121">Not supported.</span></span>  |
|<span data-ttu-id="d2497-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2497-122">Application</span></span> | <span data-ttu-id="d2497-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2497-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d2497-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2497-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="d2497-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2497-125">Request headers</span></span>
| <span data-ttu-id="d2497-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2497-126">Header</span></span>       | <span data-ttu-id="d2497-127">Значение</span><span class="sxs-lookup"><span data-stu-id="d2497-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d2497-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2497-128">Authorization</span></span>  | <span data-ttu-id="d2497-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2497-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2497-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2497-131">Request body</span></span>
<span data-ttu-id="d2497-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2497-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d2497-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2497-133">Response</span></span>
<span data-ttu-id="d2497-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d2497-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2497-136">Пример</span><span class="sxs-lookup"><span data-stu-id="d2497-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2497-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2497-137">Request</span></span>
<span data-ttu-id="d2497-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2497-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="d2497-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2497-139">Response</span></span>
<span data-ttu-id="d2497-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d2497-140">The following is an example of the response.</span></span> 

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
