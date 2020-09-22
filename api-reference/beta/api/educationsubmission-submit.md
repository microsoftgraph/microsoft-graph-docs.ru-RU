---
title: 'educationSubmission: подача'
description: Действие, которое указывает, что учащийся выполнил работу и готов к работе с назначением. Это действие может выполняться только студентом.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 948793527423a93f05bf890708651fd9e60bca56
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007268"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="a761c-104">educationSubmission: подача</span><span class="sxs-lookup"><span data-stu-id="a761c-104">educationSubmission: submit</span></span>

<span data-ttu-id="a761c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a761c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a761c-106">Действие, которое указывает, что учащийся выполнил работу и готов к работе с назначением.</span><span class="sxs-lookup"><span data-stu-id="a761c-106">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="a761c-107">Это действие может выполняться только студентом.</span><span class="sxs-lookup"><span data-stu-id="a761c-107">This action can only be taken by the student.</span></span> <span data-ttu-id="a761c-108">При этом состояние отправки будет изменено с "работает" на "Отправлено".</span><span class="sxs-lookup"><span data-stu-id="a761c-108">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="a761c-109">Во время процесса отсылки все ресурсы будут скопированы в сегмент Субмиттедресаурцес.</span><span class="sxs-lookup"><span data-stu-id="a761c-109">During the submit process, all the resources will be copied to the submittedResources bucket.</span></span> <span data-ttu-id="a761c-110">Преподаватель будет искать в списке отправленные ресурсы для ступенчатого.</span><span class="sxs-lookup"><span data-stu-id="a761c-110">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="a761c-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a761c-111">Permissions</span></span>
<span data-ttu-id="a761c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a761c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a761c-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a761c-114">Permission type</span></span>      | <span data-ttu-id="a761c-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a761c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a761c-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a761c-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="a761c-117">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a761c-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="a761c-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a761c-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a761c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a761c-119">Not supported.</span></span>  |
|<span data-ttu-id="a761c-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a761c-120">Application</span></span> | <span data-ttu-id="a761c-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a761c-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a761c-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a761c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit

```
## <a name="request-headers"></a><span data-ttu-id="a761c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a761c-123">Request headers</span></span>
| <span data-ttu-id="a761c-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a761c-124">Header</span></span>       | <span data-ttu-id="a761c-125">Значение</span><span class="sxs-lookup"><span data-stu-id="a761c-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a761c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a761c-126">Authorization</span></span>  | <span data-ttu-id="a761c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a761c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a761c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a761c-129">Request body</span></span>
<span data-ttu-id="a761c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a761c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a761c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a761c-131">Response</span></span>
<span data-ttu-id="a761c-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a761c-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a761c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="a761c-134">Example</span></span>
<span data-ttu-id="a761c-135">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="a761c-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a761c-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a761c-136">Request</span></span>
<span data-ttu-id="a761c-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a761c-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a761c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a761c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```
# <a name="c"></a>[<span data-ttu-id="a761c-139">C#</span><span class="sxs-lookup"><span data-stu-id="a761c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-submit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a761c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a761c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-submit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a761c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a761c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-submit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a761c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a761c-142">Response</span></span>
<span data-ttu-id="a761c-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a761c-143">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


