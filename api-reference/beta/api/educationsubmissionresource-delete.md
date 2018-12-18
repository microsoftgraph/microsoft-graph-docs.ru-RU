---
title: Удаление educationSubmissionResource
description: Удаляет ресурс из подачи. Это может быть выполнено только с учащегося. Если ресурс был скопирован из назначения, новую копию ресурса создается после удаления текущей копии.
author: dipakboyed
ms.openlocfilehash: d56df6cee3884556186554d9c24ae09ed802c4f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313274"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="2466f-105">Удаление educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="2466f-105">Delete educationSubmissionResource</span></span>

> <span data-ttu-id="2466f-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2466f-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2466f-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2466f-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2466f-108">Удаляет ресурс из подачи.</span><span class="sxs-lookup"><span data-stu-id="2466f-108">Deletes a resource from the submission.</span></span> <span data-ttu-id="2466f-109">Это может быть выполнено только с учащегося.</span><span class="sxs-lookup"><span data-stu-id="2466f-109">This can only be done by the student.</span></span> <span data-ttu-id="2466f-110">Если ресурс был скопирован из назначения, новую копию ресурса создается после удаления текущей копии.</span><span class="sxs-lookup"><span data-stu-id="2466f-110">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="2466f-111">Это позволяет «Сброс» ресурса в исходное состояние.</span><span class="sxs-lookup"><span data-stu-id="2466f-111">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="2466f-112">Если ресурс не был скопирован из назначения, но был добавлен из студента, ресурса просто удален.</span><span class="sxs-lookup"><span data-stu-id="2466f-112">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="2466f-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2466f-113">Permissions</span></span>
<span data-ttu-id="2466f-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2466f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2466f-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2466f-116">Permission type</span></span>      | <span data-ttu-id="2466f-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2466f-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2466f-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2466f-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="2466f-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2466f-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="2466f-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2466f-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2466f-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2466f-121">Not supported.</span></span>  |
|<span data-ttu-id="2466f-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2466f-122">Application</span></span> | <span data-ttu-id="2466f-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2466f-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2466f-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2466f-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="2466f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2466f-125">Request headers</span></span>
| <span data-ttu-id="2466f-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2466f-126">Header</span></span>       | <span data-ttu-id="2466f-127">Значение</span><span class="sxs-lookup"><span data-stu-id="2466f-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2466f-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2466f-128">Authorization</span></span>  | <span data-ttu-id="2466f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2466f-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2466f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2466f-131">Request body</span></span>
<span data-ttu-id="2466f-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2466f-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2466f-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="2466f-133">Response</span></span>
<span data-ttu-id="2466f-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2466f-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2466f-136">Пример</span><span class="sxs-lookup"><span data-stu-id="2466f-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2466f-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="2466f-137">Request</span></span>
<span data-ttu-id="2466f-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2466f-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="2466f-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="2466f-139">Response</span></span>
<span data-ttu-id="2466f-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2466f-140">The following is an example of the response.</span></span> 

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