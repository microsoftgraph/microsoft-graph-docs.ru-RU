---
title: 'educationSubmission: unsubmit'
description: 'Действие, которое указывает, что студенту требуется работать с отправкой назначения после его включения. Это действие может выполняться только студентом. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 84b3b99b6ef04585f6380c297a98a08d909ff6ac
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259486"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="cbe82-104">educationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="cbe82-104">educationSubmission: unsubmit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbe82-105">Действие, которое указывает, что студенту требуется работать с отправкой назначения после его включения.</span><span class="sxs-lookup"><span data-stu-id="cbe82-105">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="cbe82-106">Это действие может выполняться только студентом.</span><span class="sxs-lookup"><span data-stu-id="cbe82-106">This action can only be taken by the student.</span></span> <span data-ttu-id="cbe82-107">Это приведет к изменению состояния отправки с "Отправлено" на "работа".</span><span class="sxs-lookup"><span data-stu-id="cbe82-107">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="cbe82-108">Во время процесса отсылки все ресурсы будут скопированы из Субмиттедресаурцес в сегмент Воркингресаурцес.</span><span class="sxs-lookup"><span data-stu-id="cbe82-108">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="cbe82-109">Преподаватель будет искать в списке рабочие ресурсы для ступенчатого использования.</span><span class="sxs-lookup"><span data-stu-id="cbe82-109">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbe82-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cbe82-110">Permissions</span></span>
<span data-ttu-id="cbe82-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbe82-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbe82-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbe82-113">Permission type</span></span>      | <span data-ttu-id="cbe82-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbe82-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbe82-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbe82-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="cbe82-116">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbe82-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="cbe82-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbe82-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cbe82-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbe82-118">Not supported.</span></span>  |
|<span data-ttu-id="cbe82-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cbe82-119">Application</span></span> | <span data-ttu-id="cbe82-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbe82-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cbe82-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbe82-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="cbe82-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cbe82-122">Request headers</span></span>
| <span data-ttu-id="cbe82-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cbe82-123">Header</span></span>       | <span data-ttu-id="cbe82-124">Значение</span><span class="sxs-lookup"><span data-stu-id="cbe82-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cbe82-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cbe82-125">Authorization</span></span>  | <span data-ttu-id="cbe82-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbe82-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cbe82-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cbe82-128">Request body</span></span>
<span data-ttu-id="cbe82-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cbe82-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbe82-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="cbe82-130">Response</span></span>
<span data-ttu-id="cbe82-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cbe82-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbe82-133">Пример</span><span class="sxs-lookup"><span data-stu-id="cbe82-133">Example</span></span>
<span data-ttu-id="cbe82-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="cbe82-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cbe82-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbe82-135">Request</span></span>
<span data-ttu-id="cbe82-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbe82-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```

##### <a name="response"></a><span data-ttu-id="cbe82-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbe82-137">Response</span></span>
<span data-ttu-id="cbe82-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cbe82-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cbe82-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="cbe82-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cbe82-140">C#</span><span class="sxs-lookup"><span data-stu-id="cbe82-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/educationsubmission_unsubmit-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cbe82-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="cbe82-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/educationsubmission_unsubmit-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="cbe82-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cbe82-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/educationsubmission_unsubmit-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/educationsubmission-unsubmit.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationsubmission-unsubmit.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsubmission-unsubmit.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
