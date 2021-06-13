---
title: 'educationAssignment: публикация'
description: Это действие меняет состояние назначения с исходного состояния черновика на опубликованный.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3badfbf152188a0a999c41f1bcb2edffce3bf9f9
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911923"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="d2e76-103">educationAssignment: публикация</span><span class="sxs-lookup"><span data-stu-id="d2e76-103">educationAssignment: publish</span></span>

<span data-ttu-id="d2e76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2e76-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2e76-105">Это действие меняет состояние назначения с исходного состояния черновика на опубликованный.</span><span class="sxs-lookup"><span data-stu-id="d2e76-105">This action changes the state of an assignment from its original draft status to the published status.</span></span> 

<span data-ttu-id="d2e76-106">Только учитель в классе может сделать этот вызов.</span><span class="sxs-lookup"><span data-stu-id="d2e76-106">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="d2e76-107">Когда назначение находится в состоянии черновика, учащиеся не будут видеть назначение, равно как и объекты отправки.</span><span class="sxs-lookup"><span data-stu-id="d2e76-107">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="d2e76-108">При вызове этого API создаются объекты отправки и назначение отображается в списке учащегося.</span><span class="sxs-lookup"><span data-stu-id="d2e76-108">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2e76-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2e76-109">Permissions</span></span>
<span data-ttu-id="d2e76-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2e76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2e76-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2e76-112">Permission type</span></span>      | <span data-ttu-id="d2e76-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2e76-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2e76-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2e76-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="d2e76-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2e76-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d2e76-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2e76-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d2e76-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2e76-117">Not supported.</span></span>  |
|<span data-ttu-id="d2e76-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2e76-118">Application</span></span> | <span data-ttu-id="d2e76-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2e76-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d2e76-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2e76-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="d2e76-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2e76-121">Request headers</span></span>
| <span data-ttu-id="d2e76-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2e76-122">Header</span></span>       | <span data-ttu-id="d2e76-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d2e76-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d2e76-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2e76-124">Authorization</span></span>  | <span data-ttu-id="d2e76-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2e76-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2e76-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2e76-127">Request body</span></span>
<span data-ttu-id="d2e76-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2e76-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2e76-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2e76-129">Response</span></span>
<span data-ttu-id="d2e76-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d2e76-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2e76-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d2e76-132">Example</span></span>
<span data-ttu-id="d2e76-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="d2e76-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d2e76-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2e76-134">Request</span></span>
<span data-ttu-id="d2e76-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2e76-135">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2e76-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2e76-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish_2"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```
# <a name="c"></a>[<span data-ttu-id="d2e76-137">C#</span><span class="sxs-lookup"><span data-stu-id="d2e76-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2e76-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2e76-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2e76-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2e76-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2e76-140">Java</span><span class="sxs-lookup"><span data-stu-id="d2e76-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d2e76-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2e76-141">Response</span></span>
<span data-ttu-id="d2e76-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2e76-142">The following is an example of a response.</span></span> 

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
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


