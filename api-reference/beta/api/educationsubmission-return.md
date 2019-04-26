---
title: 'educationSubmission: Return'
description: Это действие делает оценку и обратную связь, связанную с этой отправкой, доступной студенту.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8d86cb72b54acae5485125e5516e494baeeaccef
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324880"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="e81fb-103">educationSubmission: Return</span><span class="sxs-lookup"><span data-stu-id="e81fb-103">educationSubmission: return</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e81fb-104">Это действие делает оценку и обратную связь, связанную с этой отправкой, доступной студенту.</span><span class="sxs-lookup"><span data-stu-id="e81fb-104">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="e81fb-105">Это приведет к изменению состояния отправки с "Отправлено" на "возвращен" и указывает на то, что обратная связь передается или выполняется ступенчатое.</span><span class="sxs-lookup"><span data-stu-id="e81fb-105">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="e81fb-106">Это действие может выполнить только преподаватель.</span><span class="sxs-lookup"><span data-stu-id="e81fb-106">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="e81fb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e81fb-107">Permissions</span></span>
<span data-ttu-id="e81fb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e81fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e81fb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e81fb-110">Permission type</span></span>      | <span data-ttu-id="e81fb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e81fb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e81fb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e81fb-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="e81fb-113">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e81fb-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="e81fb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e81fb-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e81fb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e81fb-115">Not supported.</span></span>  |
|<span data-ttu-id="e81fb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e81fb-116">Application</span></span> | <span data-ttu-id="e81fb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e81fb-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e81fb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e81fb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="e81fb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e81fb-119">Request headers</span></span>
| <span data-ttu-id="e81fb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e81fb-120">Header</span></span>       | <span data-ttu-id="e81fb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e81fb-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e81fb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e81fb-122">Authorization</span></span>  | <span data-ttu-id="e81fb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e81fb-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e81fb-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e81fb-125">Request body</span></span>
<span data-ttu-id="e81fb-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e81fb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e81fb-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="e81fb-127">Response</span></span>
<span data-ttu-id="e81fb-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e81fb-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e81fb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e81fb-130">Example</span></span>
<span data-ttu-id="e81fb-131">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="e81fb-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e81fb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e81fb-132">Request</span></span>
<span data-ttu-id="e81fb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e81fb-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="e81fb-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e81fb-134">Response</span></span>
<span data-ttu-id="e81fb-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e81fb-135">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: return",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
