---
title: 'educationSubmission: unsubmit'
description: 'Действие, которое указывает, что студента работает на отправки назначения после включения. Это действие может быть занято только учащегося. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e8ce4c5d4bf68dca22f686a1b3647c67d7836bed
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513510"
---
# <a name="educationsubmission-unsubmit"></a><span data-ttu-id="f35aa-104">educationSubmission: unsubmit</span><span class="sxs-lookup"><span data-stu-id="f35aa-104">educationSubmission: unsubmit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f35aa-105">Действие, которое указывает, что студента работает на отправки назначения после включения.</span><span class="sxs-lookup"><span data-stu-id="f35aa-105">An action that indicates that a student wants to work on the submission of the assignment after it was turned in.</span></span> <span data-ttu-id="f35aa-106">Это действие может быть занято только учащегося.</span><span class="sxs-lookup"><span data-stu-id="f35aa-106">This action can only be taken by the student.</span></span> <span data-ttu-id="f35aa-107">Состояние отправки из «отправленные» изменится на «работа».</span><span class="sxs-lookup"><span data-stu-id="f35aa-107">This will change the status of the submission from "submitted" to "working".</span></span> <span data-ttu-id="f35aa-108">Во время процесса отправки все ресурсы копируются из submittedResources интервалов workingResources.</span><span class="sxs-lookup"><span data-stu-id="f35aa-108">During the submit process, all the resources will be copied from submittedResources to the workingResources bucket.</span></span> <span data-ttu-id="f35aa-109">Преподаватель выполнит поиск в списке ресурсы рабочее для ранжирования.</span><span class="sxs-lookup"><span data-stu-id="f35aa-109">The teacher will be looking at the working resources list for grading.</span></span>

## <a name="permissions"></a><span data-ttu-id="f35aa-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f35aa-110">Permissions</span></span>
<span data-ttu-id="f35aa-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f35aa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f35aa-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f35aa-113">Permission type</span></span>      | <span data-ttu-id="f35aa-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f35aa-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f35aa-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f35aa-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="f35aa-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f35aa-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f35aa-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f35aa-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f35aa-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f35aa-118">Not supported.</span></span>  |
|<span data-ttu-id="f35aa-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f35aa-119">Application</span></span> | <span data-ttu-id="f35aa-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f35aa-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f35aa-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f35aa-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit

```
## <a name="request-headers"></a><span data-ttu-id="f35aa-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f35aa-122">Request headers</span></span>
| <span data-ttu-id="f35aa-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f35aa-123">Header</span></span>       | <span data-ttu-id="f35aa-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f35aa-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f35aa-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f35aa-125">Authorization</span></span>  | <span data-ttu-id="f35aa-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f35aa-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f35aa-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f35aa-128">Request body</span></span>
<span data-ttu-id="f35aa-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f35aa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f35aa-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="f35aa-130">Response</span></span>
<span data-ttu-id="f35aa-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f35aa-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f35aa-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f35aa-133">Example</span></span>
<span data-ttu-id="f35aa-134">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="f35aa-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f35aa-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f35aa-135">Request</span></span>
<span data-ttu-id="f35aa-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f35aa-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_unsubmit"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit
```

##### <a name="response"></a><span data-ttu-id="f35aa-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="f35aa-137">Response</span></span>
<span data-ttu-id="f35aa-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f35aa-138">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: unsubmit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-unsubmit.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
