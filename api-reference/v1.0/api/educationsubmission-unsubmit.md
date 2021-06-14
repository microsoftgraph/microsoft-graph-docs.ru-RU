---
title: 'educationSubmission: ото всех'
description: Указать, что студент хочет работать над отправкой задания после его внесения.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 152d042656f106a84fb4a89ecf8704938c251a04
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912661"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="ff232-103">educationSubmission: ото всех</span><span class="sxs-lookup"><span data-stu-id="ff232-103">educationSubmission: unsubmit</span></span>

<span data-ttu-id="ff232-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff232-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ff232-105">Указать, что студент хочет работать над отправкой задания после его внесения.</span><span class="sxs-lookup"><span data-stu-id="ff232-105">Indicate that a student wants to work on the submission of the assignment after it was turned in.</span></span> 

<span data-ttu-id="ff232-106">Это действие может быть принято только студентом.</span><span class="sxs-lookup"><span data-stu-id="ff232-106">This action can only be taken by the student.</span></span> <span data-ttu-id="ff232-107">Это изменит состояние отправки с "отправленной" на "рабочую".</span><span class="sxs-lookup"><span data-stu-id="ff232-107">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="ff232-108">Во время процесса отправки все ресурсы будут скопированы из отправкиРесурса в ведро workingResources.</span><span class="sxs-lookup"><span data-stu-id="ff232-108">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="ff232-109">Преподаватель будет искать список рабочих ресурсов для классификации.</span><span class="sxs-lookup"><span data-stu-id="ff232-109">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff232-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff232-110">Permissions</span></span>
<span data-ttu-id="ff232-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff232-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff232-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff232-113">Permission type</span></span>      | <span data-ttu-id="ff232-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff232-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff232-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff232-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="ff232-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff232-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="ff232-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff232-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ff232-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff232-118">Not supported.</span></span>  |
|<span data-ttu-id="ff232-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff232-119">Application</span></span> | <span data-ttu-id="ff232-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff232-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ff232-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff232-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="ff232-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff232-122">Request headers</span></span>
| <span data-ttu-id="ff232-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff232-123">Header</span></span>       | <span data-ttu-id="ff232-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ff232-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ff232-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ff232-125">Authorization</span></span>  | <span data-ttu-id="ff232-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff232-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ff232-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ff232-128">Request body</span></span>
<span data-ttu-id="ff232-129">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff232-129">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff232-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff232-130">Response</span></span>
<span data-ttu-id="ff232-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ff232-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff232-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ff232-133">Example</span></span>
<span data-ttu-id="ff232-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="ff232-134">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="ff232-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff232-135">Request</span></span>
<span data-ttu-id="ff232-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff232-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/unsubmit
```

### <a name="response"></a><span data-ttu-id="ff232-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff232-137">Response</span></span>
<span data-ttu-id="ff232-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ff232-138">The following is an example of the response.</span></span>

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


