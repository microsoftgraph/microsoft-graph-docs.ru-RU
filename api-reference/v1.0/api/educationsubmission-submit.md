---
title: 'educationSubmission: отправить'
description: Действие, которое указывает на то, что учащийся готов выполнять работу и готов выполнять задание. Это действие может быть принято только студентом.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1c455b022fef11b82935471a3eb90fd2b253bbd7
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912912"
---
# <a name="educationsubmission-submit"></a><span data-ttu-id="1a4e6-104">educationSubmission: отправить</span><span class="sxs-lookup"><span data-stu-id="1a4e6-104">educationSubmission: submit</span></span>

<span data-ttu-id="1a4e6-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a4e6-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1a4e6-106">Указать, что учащийся готов выполнять работу и готов выполнять задание.</span><span class="sxs-lookup"><span data-stu-id="1a4e6-106">Indicate that a student is done with the work and is ready to hand in the assignment.</span></span> 

<span data-ttu-id="1a4e6-107">Это действие может быть принято только студентом.</span><span class="sxs-lookup"><span data-stu-id="1a4e6-107">This action can only be taken by the student.</span></span> <span data-ttu-id="1a4e6-108">Это изменит состояние отправки с "рабочей" на "отправленную".</span><span class="sxs-lookup"><span data-stu-id="1a4e6-108">This will change the status of the submission from "working" to "submitted".</span></span> <span data-ttu-id="1a4e6-109">Во время процесса отправки все ресурсы будут скопированы в ведро **submittedResources.**</span><span class="sxs-lookup"><span data-stu-id="1a4e6-109">During the submit process, all the resources will be copied to the **submittedResources** bucket.</span></span> <span data-ttu-id="1a4e6-110">Учитель будет смотреть на список отправленных ресурсов для классификации.</span><span class="sxs-lookup"><span data-stu-id="1a4e6-110">The teacher will be looking at the submitted resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a4e6-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a4e6-111">Permissions</span></span>
<span data-ttu-id="1a4e6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a4e6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a4e6-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a4e6-114">Permission type</span></span>      | <span data-ttu-id="1a4e6-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a4e6-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a4e6-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a4e6-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="1a4e6-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a4e6-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="1a4e6-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a4e6-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1a4e6-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a4e6-119">Not supported.</span></span>  |
|<span data-ttu-id="1a4e6-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a4e6-120">Application</span></span> | <span data-ttu-id="1a4e6-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a4e6-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1a4e6-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a4e6-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/submit
```

## <a name="request-headers"></a><span data-ttu-id="1a4e6-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a4e6-123">Request headers</span></span>
| <span data-ttu-id="1a4e6-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1a4e6-124">Header</span></span>       | <span data-ttu-id="1a4e6-125">Значение</span><span class="sxs-lookup"><span data-stu-id="1a4e6-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1a4e6-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a4e6-126">Authorization</span></span>  | <span data-ttu-id="1a4e6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a4e6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1a4e6-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1a4e6-129">Request body</span></span>
<span data-ttu-id="1a4e6-130">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1a4e6-130">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a4e6-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a4e6-131">Response</span></span>
<span data-ttu-id="1a4e6-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1a4e6-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a4e6-134">Пример</span><span class="sxs-lookup"><span data-stu-id="1a4e6-134">Example</span></span>
<span data-ttu-id="1a4e6-135">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="1a4e6-135">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1a4e6-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a4e6-136">Request</span></span>
<span data-ttu-id="1a4e6-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a4e6-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/submit
```

### <a name="response"></a><span data-ttu-id="1a4e6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a4e6-138">Response</span></span>
<span data-ttu-id="1a4e6-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1a4e6-139">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: submit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


