---
title: 'educationSubmission: возврат'
description: Предоставление учащемуся оценки и отзывов, связанных с этим представлением.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f7c33c7bd744984ab26efb8d922716b5bb85a654
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912691"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="92d3a-103">educationSubmission: возврат</span><span class="sxs-lookup"><span data-stu-id="92d3a-103">educationSubmission: return</span></span>

<span data-ttu-id="92d3a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92d3a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="92d3a-105">Предоставление учащемуся оценки и отзывов, связанных с этим представлением.</span><span class="sxs-lookup"><span data-stu-id="92d3a-105">Make the grade and feedback associated with this submission available to the student.</span></span> 

<span data-ttu-id="92d3a-106">Это действие меняет состояние отправки с "отправленной" на "возвращенную" и указывает, что отзывы предоставлены или сделана классификация.</span><span class="sxs-lookup"><span data-stu-id="92d3a-106">This action changes the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="92d3a-107">Это действие может сделать только учитель.</span><span class="sxs-lookup"><span data-stu-id="92d3a-107">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="92d3a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="92d3a-108">Permissions</span></span>
<span data-ttu-id="92d3a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92d3a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92d3a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92d3a-111">Permission type</span></span>      | <span data-ttu-id="92d3a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="92d3a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92d3a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92d3a-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="92d3a-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92d3a-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="92d3a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92d3a-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="92d3a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92d3a-116">Not supported.</span></span>  |
|<span data-ttu-id="92d3a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92d3a-117">Application</span></span> | <span data-ttu-id="92d3a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92d3a-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="92d3a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92d3a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/return
```
## <a name="request-headers"></a><span data-ttu-id="92d3a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="92d3a-120">Request headers</span></span>
| <span data-ttu-id="92d3a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92d3a-121">Header</span></span>       | <span data-ttu-id="92d3a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="92d3a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="92d3a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92d3a-123">Authorization</span></span>  | <span data-ttu-id="92d3a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92d3a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="92d3a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="92d3a-126">Request body</span></span>
<span data-ttu-id="92d3a-127">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="92d3a-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92d3a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="92d3a-128">Response</span></span>
<span data-ttu-id="92d3a-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="92d3a-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92d3a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="92d3a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="92d3a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="92d3a-132">Request</span></span>
<span data-ttu-id="92d3a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92d3a-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/return
```

### <a name="response"></a><span data-ttu-id="92d3a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="92d3a-134">Response</span></span>
<span data-ttu-id="92d3a-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="92d3a-135">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


