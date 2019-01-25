---
title: 'educationSubmission: возврата'
description: Это действие делает марки и отзыв, связанный с этой отправки доступные студента.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b1772788230b5220b3bdc6813b122d1158e26ab2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511242"
---
# <a name="educationsubmission-return"></a><span data-ttu-id="bd703-103">educationSubmission: возврата</span><span class="sxs-lookup"><span data-stu-id="bd703-103">educationSubmission: return</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd703-104">Это действие делает марки и отзыв, связанный с этой отправки доступные студента.</span><span class="sxs-lookup"><span data-stu-id="bd703-104">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="bd703-105">Это изменение состояния подачи из «отправленные» «вернуть» и указывает на то, что обратной связи или оценка успеваемости выполняется.</span><span class="sxs-lookup"><span data-stu-id="bd703-105">This will change the status of the submission from "submitted" to "returned" and indicates that feedback is provided or grading is done.</span></span> <span data-ttu-id="bd703-106">Это действие можно выполнить только с преподаватель.</span><span class="sxs-lookup"><span data-stu-id="bd703-106">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd703-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd703-107">Permissions</span></span>
<span data-ttu-id="bd703-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd703-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd703-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd703-110">Permission type</span></span>      | <span data-ttu-id="bd703-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd703-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd703-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd703-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="bd703-113">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd703-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="bd703-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd703-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bd703-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd703-115">Not supported.</span></span>  |
|<span data-ttu-id="bd703-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd703-116">Application</span></span> | <span data-ttu-id="bd703-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd703-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bd703-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd703-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/return

```
## <a name="request-headers"></a><span data-ttu-id="bd703-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd703-119">Request headers</span></span>
| <span data-ttu-id="bd703-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd703-120">Header</span></span>       | <span data-ttu-id="bd703-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bd703-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bd703-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd703-122">Authorization</span></span>  | <span data-ttu-id="bd703-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd703-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bd703-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd703-125">Request body</span></span>
<span data-ttu-id="bd703-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd703-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd703-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd703-127">Response</span></span>
<span data-ttu-id="bd703-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bd703-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd703-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bd703-130">Example</span></span>
<span data-ttu-id="bd703-131">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="bd703-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bd703-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd703-132">Request</span></span>
<span data-ttu-id="bd703-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd703-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/return
```

##### <a name="response"></a><span data-ttu-id="bd703-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="bd703-134">Response</span></span>
<span data-ttu-id="bd703-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd703-135">The following is an example of the response.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-return.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
