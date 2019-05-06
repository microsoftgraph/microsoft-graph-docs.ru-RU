---
title: Удаление Едукатионсубмиссионресаурце
description: Удаляет ресурс из отправки. Это может сделать только студентом. Если ресурс был скопирован из назначения, то после удаления текущей копии будет создан новый экземпляр ресурса.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 056f09adb9bb36a38d613edaf8d0c1220d69bcb3
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587786"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="72682-105">Удаление Едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="72682-105">Delete educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72682-106">Удаляет ресурс из отправки.</span><span class="sxs-lookup"><span data-stu-id="72682-106">Deletes a resource from the submission.</span></span> <span data-ttu-id="72682-107">Это может сделать только студентом.</span><span class="sxs-lookup"><span data-stu-id="72682-107">This can only be done by the student.</span></span> <span data-ttu-id="72682-108">Если ресурс был скопирован из назначения, то после удаления текущей копии будет создан новый экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="72682-108">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="72682-109">Это позволяет «сбросить» ресурс в исходное состояние.</span><span class="sxs-lookup"><span data-stu-id="72682-109">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="72682-110">Если ресурс не был скопирован из назначения, но добавлен из учащегося, ресурс просто удаляется.</span><span class="sxs-lookup"><span data-stu-id="72682-110">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="72682-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72682-111">Permissions</span></span>
<span data-ttu-id="72682-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72682-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72682-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72682-114">Permission type</span></span>      | <span data-ttu-id="72682-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72682-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72682-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72682-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="72682-117">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72682-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="72682-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72682-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="72682-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72682-119">Not supported.</span></span>  |
|<span data-ttu-id="72682-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72682-120">Application</span></span> | <span data-ttu-id="72682-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72682-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="72682-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72682-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="72682-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72682-123">Request headers</span></span>
| <span data-ttu-id="72682-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72682-124">Header</span></span>       | <span data-ttu-id="72682-125">Значение</span><span class="sxs-lookup"><span data-stu-id="72682-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="72682-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72682-126">Authorization</span></span>  | <span data-ttu-id="72682-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72682-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="72682-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72682-129">Request body</span></span>
<span data-ttu-id="72682-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72682-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="72682-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="72682-131">Response</span></span>
<span data-ttu-id="72682-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="72682-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72682-134">Пример</span><span class="sxs-lookup"><span data-stu-id="72682-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72682-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="72682-135">Request</span></span>
<span data-ttu-id="72682-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72682-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="72682-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="72682-137">Response</span></span>
<span data-ttu-id="72682-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="72682-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="72682-139">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="72682-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="72682-140">Языках</span><span class="sxs-lookup"><span data-stu-id="72682-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_educationsubmissionresource-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72682-141">Язык</span><span class="sxs-lookup"><span data-stu-id="72682-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_educationsubmissionresource-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/educationsubmissionresource-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsubmissionresource-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
