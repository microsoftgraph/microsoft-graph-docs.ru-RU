---
title: 'educationAssignment: публикация'
description: Это действие изменяет состояние назначения его исходное состояние черновика для опубликованного состояние. Только преподаватель в классе можно позвонить. После назначения находится в состоянии черновиков, студентов не отображается как назначения, а также будет ли любые объекты отправки. При вызове этот интерфейс API для создания объектов отправки и назначения в списке учащегося.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: bac9c38d5fbd2ce80693a468c0a2d229085f32cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508715"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="e10c7-106">educationAssignment: публикация</span><span class="sxs-lookup"><span data-stu-id="e10c7-106">educationAssignment: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e10c7-107">Это действие изменяет состояние назначения его исходное состояние черновика для опубликованного состояние.</span><span class="sxs-lookup"><span data-stu-id="e10c7-107">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="e10c7-108">Только преподаватель в классе можно позвонить.</span><span class="sxs-lookup"><span data-stu-id="e10c7-108">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="e10c7-109">После назначения находится в состоянии черновиков, студентов не отображается как назначения, а также будет ли любые объекты отправки.</span><span class="sxs-lookup"><span data-stu-id="e10c7-109">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="e10c7-110">При вызове этот интерфейс API для создания объектов отправки и назначения в списке учащегося.</span><span class="sxs-lookup"><span data-stu-id="e10c7-110">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="e10c7-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e10c7-111">Permissions</span></span>
<span data-ttu-id="e10c7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e10c7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e10c7-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e10c7-114">Permission type</span></span>      | <span data-ttu-id="e10c7-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e10c7-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e10c7-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e10c7-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="e10c7-117">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e10c7-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e10c7-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e10c7-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e10c7-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e10c7-119">Not supported.</span></span>  |
|<span data-ttu-id="e10c7-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e10c7-120">Application</span></span> | <span data-ttu-id="e10c7-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e10c7-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e10c7-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e10c7-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="e10c7-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e10c7-123">Request headers</span></span>
| <span data-ttu-id="e10c7-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e10c7-124">Header</span></span>       | <span data-ttu-id="e10c7-125">Значение</span><span class="sxs-lookup"><span data-stu-id="e10c7-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e10c7-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e10c7-126">Authorization</span></span>  | <span data-ttu-id="e10c7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e10c7-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e10c7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e10c7-129">Request body</span></span>
<span data-ttu-id="e10c7-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e10c7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e10c7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e10c7-131">Response</span></span>
<span data-ttu-id="e10c7-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e10c7-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e10c7-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e10c7-134">Example</span></span>
<span data-ttu-id="e10c7-135">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="e10c7-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e10c7-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="e10c7-136">Request</span></span>
<span data-ttu-id="e10c7-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e10c7-137">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```

##### <a name="response"></a><span data-ttu-id="e10c7-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="e10c7-138">Response</span></span>
<span data-ttu-id="e10c7-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e10c7-139">The following is an example of a response.</span></span> 

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
    "Error: /api-reference/beta/api/educationassignment-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
