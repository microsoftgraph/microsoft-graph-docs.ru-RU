---
title: 'educationSubmission: возврат'
description: Это действие делает оценку и отзывы, связанные с этим представлением, доступными для учащегося.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: da0f7f6c92ce5c0782f076ad10280355e4a009c0
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787291"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="3e55f-103">educationSubmission: возврат</span><span class="sxs-lookup"><span data-stu-id="3e55f-103">educationSubmission: return</span></span>

<span data-ttu-id="3e55f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e55f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e55f-105">Это действие делает оценку и отзывы, связанные с этим представлением, доступными для учащегося.</span><span class="sxs-lookup"><span data-stu-id="3e55f-105">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="3e55f-106">Это изменит состояние отправки с "отправленной" на "возвращенную" и указывает на то, что обратная связь предоставлена или сделана классификация.</span><span class="sxs-lookup"><span data-stu-id="3e55f-106">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="3e55f-107">Это действие может сделать только учитель.</span><span class="sxs-lookup"><span data-stu-id="3e55f-107">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e55f-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e55f-108">Permissions</span></span>
<span data-ttu-id="3e55f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e55f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e55f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e55f-111">Permission type</span></span>      | <span data-ttu-id="3e55f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e55f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e55f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e55f-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="3e55f-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3e55f-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="3e55f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e55f-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3e55f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e55f-116">Not supported.</span></span>  |
|<span data-ttu-id="3e55f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e55f-117">Application</span></span> | <span data-ttu-id="3e55f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e55f-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3e55f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e55f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return
```
## <a name="request-headers"></a><span data-ttu-id="3e55f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e55f-120">Request headers</span></span>
| <span data-ttu-id="3e55f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e55f-121">Header</span></span>       | <span data-ttu-id="3e55f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3e55f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3e55f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e55f-123">Authorization</span></span>  | <span data-ttu-id="3e55f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e55f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3e55f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e55f-126">Request body</span></span>
<span data-ttu-id="3e55f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e55f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e55f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e55f-128">Response</span></span>
<span data-ttu-id="3e55f-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3e55f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e55f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3e55f-131">Example</span></span>
<span data-ttu-id="3e55f-132">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="3e55f-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3e55f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e55f-133">Request</span></span>
<span data-ttu-id="3e55f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e55f-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3e55f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e55f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```
# <a name="c"></a>[<span data-ttu-id="3e55f-136">C#</span><span class="sxs-lookup"><span data-stu-id="3e55f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-return-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e55f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e55f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-return-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e55f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e55f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-return-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3e55f-139">Java</span><span class="sxs-lookup"><span data-stu-id="3e55f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-return-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3e55f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e55f-140">Response</span></span>
<span data-ttu-id="3e55f-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3e55f-141">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


