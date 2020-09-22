---
title: 'educationAssignment: публикация'
description: Это действие изменяет состояние назначения с исходного черновика на опубликованное. Только преподаватель в классе может совершать этот вызов. Если для назначения выбран статус черновика, студенты не увидят назначение и не будут иметь объектов отправки. При вызове этого API создаются объекты отправки, а Назначение отображается в списке учащихся.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8bd23a420c5f4ca3b5e8a666b8b4a153e602fb34
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007765"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="98708-106">educationAssignment: публикация</span><span class="sxs-lookup"><span data-stu-id="98708-106">educationAssignment: publish</span></span>

<span data-ttu-id="98708-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98708-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98708-108">Это действие изменяет состояние назначения с исходного черновика на опубликованное.</span><span class="sxs-lookup"><span data-stu-id="98708-108">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="98708-109">Только преподаватель в классе может совершать этот вызов.</span><span class="sxs-lookup"><span data-stu-id="98708-109">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="98708-110">Если для назначения выбран статус черновика, студенты не увидят назначение и не будут иметь объектов отправки.</span><span class="sxs-lookup"><span data-stu-id="98708-110">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="98708-111">При вызове этого API создаются объекты отправки, а Назначение отображается в списке учащихся.</span><span class="sxs-lookup"><span data-stu-id="98708-111">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="98708-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98708-112">Permissions</span></span>
<span data-ttu-id="98708-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98708-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98708-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98708-115">Permission type</span></span>      | <span data-ttu-id="98708-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98708-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98708-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98708-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="98708-118">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98708-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="98708-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98708-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="98708-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98708-120">Not supported.</span></span>  |
|<span data-ttu-id="98708-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98708-121">Application</span></span> | <span data-ttu-id="98708-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98708-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="98708-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98708-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="98708-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98708-124">Request headers</span></span>
| <span data-ttu-id="98708-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98708-125">Header</span></span>       | <span data-ttu-id="98708-126">Значение</span><span class="sxs-lookup"><span data-stu-id="98708-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="98708-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98708-127">Authorization</span></span>  | <span data-ttu-id="98708-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98708-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="98708-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="98708-130">Request body</span></span>
<span data-ttu-id="98708-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98708-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98708-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="98708-132">Response</span></span>
<span data-ttu-id="98708-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="98708-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98708-135">Пример</span><span class="sxs-lookup"><span data-stu-id="98708-135">Example</span></span>
<span data-ttu-id="98708-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="98708-136">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="98708-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="98708-137">Request</span></span>
<span data-ttu-id="98708-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98708-138">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="98708-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="98708-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```
# <a name="c"></a>[<span data-ttu-id="98708-140">C#</span><span class="sxs-lookup"><span data-stu-id="98708-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98708-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98708-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98708-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98708-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="98708-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="98708-143">Response</span></span>
<span data-ttu-id="98708-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="98708-144">The following is an example of a response.</span></span> 

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


