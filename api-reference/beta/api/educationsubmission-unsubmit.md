---
title: 'educationSubmission: ото всех'
description: 'Действие, которое указывает на то, что студент хочет работать над отправкой назначения после его внесения. Это действие может быть принято только студентом. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 23f6a2ec01dde64ec12ff8f3a378c40b1b3fd3cb
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787277"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="a60b8-104">educationSubmission: ото всех</span><span class="sxs-lookup"><span data-stu-id="a60b8-104">educationSubmission: unsubmit</span></span>

<span data-ttu-id="a60b8-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a60b8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a60b8-106">Действие, которое указывает на то, что студент хочет работать над отправкой назначения после его внесения.</span><span class="sxs-lookup"><span data-stu-id="a60b8-106">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="a60b8-107">Это действие может быть принято только студентом.</span><span class="sxs-lookup"><span data-stu-id="a60b8-107">This action can only be taken by the student.</span></span> <span data-ttu-id="a60b8-108">Это изменит состояние отправки с "отправленной" на "рабочую".</span><span class="sxs-lookup"><span data-stu-id="a60b8-108">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="a60b8-109">Во время процесса отправки все ресурсы будут скопированы из отправкиРесурса в ведро workingResources.</span><span class="sxs-lookup"><span data-stu-id="a60b8-109">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="a60b8-110">Преподаватель будет искать список рабочих ресурсов для классификации.</span><span class="sxs-lookup"><span data-stu-id="a60b8-110">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="a60b8-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a60b8-111">Permissions</span></span>
<span data-ttu-id="a60b8-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a60b8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a60b8-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a60b8-114">Permission type</span></span>      | <span data-ttu-id="a60b8-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a60b8-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a60b8-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a60b8-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="a60b8-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a60b8-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="a60b8-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a60b8-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a60b8-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a60b8-119">Not supported.</span></span>  |
|<span data-ttu-id="a60b8-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a60b8-120">Application</span></span> | <span data-ttu-id="a60b8-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a60b8-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a60b8-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a60b8-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit
```
## <a name="request-headers"></a><span data-ttu-id="a60b8-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a60b8-123">Request headers</span></span>
| <span data-ttu-id="a60b8-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a60b8-124">Header</span></span>       | <span data-ttu-id="a60b8-125">Значение</span><span class="sxs-lookup"><span data-stu-id="a60b8-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a60b8-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a60b8-126">Authorization</span></span>  | <span data-ttu-id="a60b8-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a60b8-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a60b8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a60b8-129">Request body</span></span>
<span data-ttu-id="a60b8-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a60b8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a60b8-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a60b8-131">Response</span></span>
<span data-ttu-id="a60b8-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a60b8-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a60b8-134">Пример</span><span class="sxs-lookup"><span data-stu-id="a60b8-134">Example</span></span>
<span data-ttu-id="a60b8-135">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="a60b8-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a60b8-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a60b8-136">Request</span></span>
<span data-ttu-id="a60b8-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a60b8-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a60b8-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a60b8-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```
# <a name="c"></a>[<span data-ttu-id="a60b8-139">C#</span><span class="sxs-lookup"><span data-stu-id="a60b8-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-unsubmit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a60b8-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a60b8-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-unsubmit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a60b8-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a60b8-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-unsubmit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a60b8-142">Java</span><span class="sxs-lookup"><span data-stu-id="a60b8-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-unsubmit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a60b8-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="a60b8-143">Response</span></span>
<span data-ttu-id="a60b8-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a60b8-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: unsubmit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


