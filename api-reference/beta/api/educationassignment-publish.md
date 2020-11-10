---
title: 'educationAssignment: публикация'
description: Это действие изменяет состояние назначения с исходного черновика на опубликованное. Только преподаватель в классе может совершать этот вызов. Если для назначения выбран статус черновика, студенты не увидят назначение и не будут иметь объектов отправки. При вызове этого API создаются объекты отправки, а Назначение отображается в списке учащихся.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 40e32d07e89d870a12143b4b970f8a8520b508c0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966531"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="3cdf4-106">educationAssignment: публикация</span><span class="sxs-lookup"><span data-stu-id="3cdf4-106">educationAssignment: publish</span></span>

<span data-ttu-id="3cdf4-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cdf4-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cdf4-108">Это действие изменяет состояние назначения с исходного черновика на опубликованное.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-108">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="3cdf4-109">Только преподаватель в классе может совершать этот вызов.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-109">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="3cdf4-110">Если для назначения выбран статус черновика, студенты не увидят назначение и не будут иметь объектов отправки.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-110">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="3cdf4-111">При вызове этого API создаются объекты отправки, а Назначение отображается в списке учащихся.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-111">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cdf4-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3cdf4-112">Permissions</span></span>
<span data-ttu-id="3cdf4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cdf4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cdf4-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cdf4-115">Permission type</span></span>      | <span data-ttu-id="3cdf4-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cdf4-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cdf4-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cdf4-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="3cdf4-118">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3cdf4-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="3cdf4-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cdf4-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3cdf4-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-120">Not supported.</span></span>  |
|<span data-ttu-id="3cdf4-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3cdf4-121">Application</span></span> | <span data-ttu-id="3cdf4-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3cdf4-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cdf4-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="3cdf4-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3cdf4-124">Request headers</span></span>
| <span data-ttu-id="3cdf4-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3cdf4-125">Header</span></span>       | <span data-ttu-id="3cdf4-126">Значение</span><span class="sxs-lookup"><span data-stu-id="3cdf4-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3cdf4-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3cdf4-127">Authorization</span></span>  | <span data-ttu-id="3cdf4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3cdf4-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3cdf4-130">Request body</span></span>
<span data-ttu-id="3cdf4-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cdf4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cdf4-132">Response</span></span>
<span data-ttu-id="3cdf4-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cdf4-135">Пример</span><span class="sxs-lookup"><span data-stu-id="3cdf4-135">Example</span></span>
<span data-ttu-id="3cdf4-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3cdf4-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="3cdf4-137">Request</span></span>
<span data-ttu-id="3cdf4-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-138">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3cdf4-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cdf4-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```
# <a name="c"></a>[<span data-ttu-id="3cdf4-140">C#</span><span class="sxs-lookup"><span data-stu-id="3cdf4-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cdf4-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cdf4-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cdf4-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cdf4-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cdf4-143">Java</span><span class="sxs-lookup"><span data-stu-id="3cdf4-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3cdf4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="3cdf4-144">Response</span></span>
<span data-ttu-id="3cdf4-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3cdf4-145">The following is an example of a response.</span></span> 

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
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


