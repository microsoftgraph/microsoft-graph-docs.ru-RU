---
title: Удаление educationSubmissionResource
description: Удаляет ресурс из подачи. Это может быть выполнено только с учащегося. Если ресурс был скопирован из назначения, новую копию ресурса создается после удаления текущей копии.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 657e05a5a60dd90c8fd0c769b7d978c4be617201
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945729"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="d0c2e-105">Удаление educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="d0c2e-105">Delete educationSubmissionResource</span></span>

> <span data-ttu-id="d0c2e-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d0c2e-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0c2e-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0c2e-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0c2e-108">Удаляет ресурс из подачи.</span><span class="sxs-lookup"><span data-stu-id="d0c2e-108">Deletes a resource from the submission.</span></span> <span data-ttu-id="d0c2e-109">Это может быть выполнено только с учащегося.</span><span class="sxs-lookup"><span data-stu-id="d0c2e-109">This can only be done by the student.</span></span> <span data-ttu-id="d0c2e-110">Если ресурс был скопирован из назначения, новую копию ресурса создается после удаления текущей копии.</span><span class="sxs-lookup"><span data-stu-id="d0c2e-110">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="d0c2e-111">Это позволяет «Сброс» ресурса в исходное состояние.</span><span class="sxs-lookup"><span data-stu-id="d0c2e-111">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="d0c2e-112">Если ресурс не был скопирован из назначения, но был добавлен из студента, ресурса просто удален.</span><span class="sxs-lookup"><span data-stu-id="d0c2e-112">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0c2e-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0c2e-113">Permissions</span></span>
<span data-ttu-id="d0c2e-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0c2e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0c2e-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0c2e-116">Permission type</span></span>      | <span data-ttu-id="d0c2e-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0c2e-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0c2e-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0c2e-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="d0c2e-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d0c2e-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d0c2e-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0c2e-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d0c2e-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0c2e-121">Not supported.</span></span>  |
|<span data-ttu-id="d0c2e-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0c2e-122">Application</span></span> | <span data-ttu-id="d0c2e-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0c2e-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d0c2e-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0c2e-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="d0c2e-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0c2e-125">Request headers</span></span>
| <span data-ttu-id="d0c2e-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0c2e-126">Header</span></span>       | <span data-ttu-id="d0c2e-127">Значение</span><span class="sxs-lookup"><span data-stu-id="d0c2e-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d0c2e-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0c2e-128">Authorization</span></span>  | <span data-ttu-id="d0c2e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0c2e-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d0c2e-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d0c2e-131">Request body</span></span>
<span data-ttu-id="d0c2e-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d0c2e-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d0c2e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0c2e-133">Response</span></span>
<span data-ttu-id="d0c2e-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d0c2e-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0c2e-136">Пример</span><span class="sxs-lookup"><span data-stu-id="d0c2e-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0c2e-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0c2e-137">Request</span></span>
<span data-ttu-id="d0c2e-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0c2e-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="d0c2e-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="d0c2e-139">Response</span></span>
<span data-ttu-id="d0c2e-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d0c2e-140">The following is an example of the response.</span></span> 

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
