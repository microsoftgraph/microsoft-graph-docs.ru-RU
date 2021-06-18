---
title: 'educationSubmission: ото всех'
description: Указать, что студент хочет работать над отправкой задания после его внесения.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4ddad6241c4e6c7820db143e93064b4570d68e49
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993293"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="0b479-103">educationSubmission: ото всех</span><span class="sxs-lookup"><span data-stu-id="0b479-103">educationSubmission: unsubmit</span></span>

<span data-ttu-id="0b479-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b479-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b479-105">Указать, что студент хочет работать над отправкой задания после его внесения.</span><span class="sxs-lookup"><span data-stu-id="0b479-105">Indicate that a student wants to work on the submission of the assignment after it was turned in.</span></span> 

<span data-ttu-id="0b479-106">Это действие может быть принято только студентом.</span><span class="sxs-lookup"><span data-stu-id="0b479-106">This action can only be taken by the student.</span></span> <span data-ttu-id="0b479-107">Это изменит состояние отправки с "отправленной" на "рабочую".</span><span class="sxs-lookup"><span data-stu-id="0b479-107">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="0b479-108">Во время процесса отправки все ресурсы будут скопированы из отправкиРесурса в ведро workingResources.</span><span class="sxs-lookup"><span data-stu-id="0b479-108">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="0b479-109">Преподаватель будет искать список рабочих ресурсов для классификации.</span><span class="sxs-lookup"><span data-stu-id="0b479-109">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b479-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b479-110">Permissions</span></span>
<span data-ttu-id="0b479-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b479-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b479-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b479-113">Permission type</span></span>      | <span data-ttu-id="0b479-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b479-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b479-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b479-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="0b479-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0b479-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="0b479-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b479-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0b479-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b479-118">Not supported.</span></span>  |
|<span data-ttu-id="0b479-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b479-119">Application</span></span> | <span data-ttu-id="0b479-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b479-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0b479-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b479-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="0b479-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b479-122">Request headers</span></span>
| <span data-ttu-id="0b479-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b479-123">Header</span></span>       | <span data-ttu-id="0b479-124">Значение</span><span class="sxs-lookup"><span data-stu-id="0b479-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0b479-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b479-125">Authorization</span></span>  | <span data-ttu-id="0b479-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b479-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0b479-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b479-128">Request body</span></span>
<span data-ttu-id="0b479-129">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b479-129">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b479-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b479-130">Response</span></span>
<span data-ttu-id="0b479-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0b479-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b479-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0b479-133">Example</span></span>
<span data-ttu-id="0b479-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="0b479-134">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="0b479-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b479-135">Request</span></span>
<span data-ttu-id="0b479-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b479-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0b479-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b479-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/unsubmit
```
# <a name="c"></a>[<span data-ttu-id="0b479-138">C#</span><span class="sxs-lookup"><span data-stu-id="0b479-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-unsubmit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b479-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b479-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-unsubmit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b479-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b479-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-unsubmit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b479-141">Java</span><span class="sxs-lookup"><span data-stu-id="0b479-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-unsubmit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0b479-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b479-142">Response</span></span>
<span data-ttu-id="0b479-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0b479-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content

{
}
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


