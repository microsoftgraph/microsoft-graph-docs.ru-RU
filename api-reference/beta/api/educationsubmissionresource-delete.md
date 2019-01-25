---
title: Удаление educationSubmissionResource
description: Удаляет ресурс из подачи. Это может быть выполнено только с учащегося. Если ресурс был скопирован из назначения, новую копию ресурса создается после удаления текущей копии.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a735cb1451e8d3eb8df13e6fa395c3e02393f451
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518984"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="1af5d-105">Удаление educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="1af5d-105">Delete educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1af5d-106">Удаляет ресурс из подачи.</span><span class="sxs-lookup"><span data-stu-id="1af5d-106">Deletes a resource from the submission.</span></span> <span data-ttu-id="1af5d-107">Это может быть выполнено только с учащегося.</span><span class="sxs-lookup"><span data-stu-id="1af5d-107">This can only be done by the student.</span></span> <span data-ttu-id="1af5d-108">Если ресурс был скопирован из назначения, новую копию ресурса создается после удаления текущей копии.</span><span class="sxs-lookup"><span data-stu-id="1af5d-108">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="1af5d-109">Это позволяет «Сброс» ресурса в исходное состояние.</span><span class="sxs-lookup"><span data-stu-id="1af5d-109">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="1af5d-110">Если ресурс не был скопирован из назначения, но был добавлен из студента, ресурса просто удален.</span><span class="sxs-lookup"><span data-stu-id="1af5d-110">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="1af5d-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1af5d-111">Permissions</span></span>
<span data-ttu-id="1af5d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1af5d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1af5d-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1af5d-114">Permission type</span></span>      | <span data-ttu-id="1af5d-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1af5d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1af5d-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1af5d-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="1af5d-117">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1af5d-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="1af5d-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1af5d-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1af5d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1af5d-119">Not supported.</span></span>  |
|<span data-ttu-id="1af5d-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1af5d-120">Application</span></span> | <span data-ttu-id="1af5d-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1af5d-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1af5d-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1af5d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="1af5d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1af5d-123">Request headers</span></span>
| <span data-ttu-id="1af5d-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1af5d-124">Header</span></span>       | <span data-ttu-id="1af5d-125">Значение</span><span class="sxs-lookup"><span data-stu-id="1af5d-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1af5d-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1af5d-126">Authorization</span></span>  | <span data-ttu-id="1af5d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1af5d-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1af5d-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1af5d-129">Request body</span></span>
<span data-ttu-id="1af5d-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1af5d-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1af5d-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="1af5d-131">Response</span></span>
<span data-ttu-id="1af5d-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1af5d-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1af5d-134">Пример</span><span class="sxs-lookup"><span data-stu-id="1af5d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1af5d-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="1af5d-135">Request</span></span>
<span data-ttu-id="1af5d-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1af5d-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="1af5d-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="1af5d-137">Response</span></span>
<span data-ttu-id="1af5d-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1af5d-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmissionresource-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
