---
title: 'educationSubmission: unsubmit'
description: 'Действие, которое указывает, что студенту требуется работать с отправкой назначения после его включения. Это действие может выполняться только студентом. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 24868993badf2b0788e35f015e8ceea0ca7361d0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955421"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="09447-104">educationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="09447-104">educationSubmission: unsubmit</span></span>

<span data-ttu-id="09447-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09447-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09447-106">Действие, которое указывает, что студенту требуется работать с отправкой назначения после его включения.</span><span class="sxs-lookup"><span data-stu-id="09447-106">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="09447-107">Это действие может выполняться только студентом.</span><span class="sxs-lookup"><span data-stu-id="09447-107">This action can only be taken by the student.</span></span> <span data-ttu-id="09447-108">Это приведет к изменению состояния отправки с "Отправлено" на "работа".</span><span class="sxs-lookup"><span data-stu-id="09447-108">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="09447-109">Во время процесса отсылки все ресурсы будут скопированы из Субмиттедресаурцес в сегмент Воркингресаурцес.</span><span class="sxs-lookup"><span data-stu-id="09447-109">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="09447-110">Преподаватель будет искать в списке рабочие ресурсы для ступенчатого использования.</span><span class="sxs-lookup"><span data-stu-id="09447-110">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="09447-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="09447-111">Permissions</span></span>
<span data-ttu-id="09447-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09447-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09447-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09447-114">Permission type</span></span>      | <span data-ttu-id="09447-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="09447-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09447-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09447-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="09447-117">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09447-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="09447-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09447-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="09447-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09447-119">Not supported.</span></span>  |
|<span data-ttu-id="09447-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09447-120">Application</span></span> | <span data-ttu-id="09447-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09447-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="09447-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09447-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="09447-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="09447-123">Request headers</span></span>
| <span data-ttu-id="09447-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09447-124">Header</span></span>       | <span data-ttu-id="09447-125">Значение</span><span class="sxs-lookup"><span data-stu-id="09447-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="09447-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="09447-126">Authorization</span></span>  | <span data-ttu-id="09447-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09447-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="09447-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09447-129">Request body</span></span>
<span data-ttu-id="09447-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="09447-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09447-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="09447-131">Response</span></span>
<span data-ttu-id="09447-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="09447-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09447-134">Пример</span><span class="sxs-lookup"><span data-stu-id="09447-134">Example</span></span>
<span data-ttu-id="09447-135">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="09447-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="09447-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="09447-136">Request</span></span>
<span data-ttu-id="09447-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09447-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="09447-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="09447-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```
# <a name="c"></a>[<span data-ttu-id="09447-139">C#</span><span class="sxs-lookup"><span data-stu-id="09447-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-unsubmit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="09447-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09447-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-unsubmit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="09447-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09447-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-unsubmit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="09447-142">Java</span><span class="sxs-lookup"><span data-stu-id="09447-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-unsubmit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="09447-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="09447-143">Response</span></span>
<span data-ttu-id="09447-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="09447-144">The following is an example of the response.</span></span>

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


