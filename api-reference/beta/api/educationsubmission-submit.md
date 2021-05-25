---
title: 'educationSubmission: отправить'
description: Действие, которое указывает на то, что учащийся готов выполнять работу и готов выполнять задание. Это действие может быть принято только студентом.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b6a7752ed51052adc1cf1420ec566c0ec2fbafac
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645404"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="b154c-104">educationSubmission: отправить</span><span class="sxs-lookup"><span data-stu-id="b154c-104">educationSubmission: submit</span></span>

<span data-ttu-id="b154c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b154c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b154c-106">Действие, которое указывает на то, что учащийся готов выполнять работу и готов выполнять задание.</span><span class="sxs-lookup"><span data-stu-id="b154c-106">An action that indicates that a student is done with the work and is ready to hand in the assignment.</span></span> <span data-ttu-id="b154c-107">Это действие может быть принято только студентом.</span><span class="sxs-lookup"><span data-stu-id="b154c-107">This action can only be taken by the student.</span></span> <span data-ttu-id="b154c-108">Это изменит состояние отправки с "рабочей" на "отправленную".</span><span class="sxs-lookup"><span data-stu-id="b154c-108">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="b154c-109">Во время процесса отправки все ресурсы будут скопированы в ведро **submittedResources.**</span><span class="sxs-lookup"><span data-stu-id="b154c-109">During the submit process, all the resources will be copied to the **submittedResources** bucket.</span></span> <span data-ttu-id="b154c-110">Учитель будет смотреть на список отправленных ресурсов для классификации.</span><span class="sxs-lookup"><span data-stu-id="b154c-110">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="b154c-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b154c-111">Permissions</span></span>
<span data-ttu-id="b154c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b154c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b154c-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b154c-114">Permission type</span></span>      | <span data-ttu-id="b154c-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b154c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b154c-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b154c-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="b154c-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b154c-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="b154c-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b154c-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b154c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b154c-119">Not supported.</span></span>  |
|<span data-ttu-id="b154c-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b154c-120">Application</span></span> | <span data-ttu-id="b154c-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b154c-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b154c-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b154c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit
```

## <a name="request-headers"></a><span data-ttu-id="b154c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b154c-123">Request headers</span></span>
| <span data-ttu-id="b154c-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b154c-124">Header</span></span>       | <span data-ttu-id="b154c-125">Значение</span><span class="sxs-lookup"><span data-stu-id="b154c-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b154c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b154c-126">Authorization</span></span>  | <span data-ttu-id="b154c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b154c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b154c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b154c-129">Request body</span></span>
<span data-ttu-id="b154c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b154c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b154c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="b154c-131">Response</span></span>
<span data-ttu-id="b154c-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b154c-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b154c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="b154c-134">Example</span></span>
<span data-ttu-id="b154c-135">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b154c-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b154c-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="b154c-136">Request</span></span>
<span data-ttu-id="b154c-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b154c-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b154c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="b154c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submit
```
# <a name="c"></a>[<span data-ttu-id="b154c-139">C#</span><span class="sxs-lookup"><span data-stu-id="b154c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-submit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b154c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b154c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-submit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b154c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b154c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-submit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b154c-142">Java</span><span class="sxs-lookup"><span data-stu-id="b154c-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-submit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b154c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b154c-143">Response</span></span>
<span data-ttu-id="b154c-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b154c-144">The following is an example of the response.</span></span>

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


