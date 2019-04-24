---
title: 'educationAssignment: публикация'
description: Это действие изменяет состояние назначения с исходного черновика на опубликованное. Только преподаватель в классе может совершать этот вызов. Если для назначения выбран статус черновика, студенты не увидят назначение и не будут иметь объектов отправки. При вызове этого API создаются объекты отправки, а Назначение отображается в списке учащихся.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: bac9c38d5fbd2ce80693a468c0a2d229085f32cd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458189"
---
# <a name="educationassignment-publish"></a><span data-ttu-id="86ed0-106">educationAssignment: публикация</span><span class="sxs-lookup"><span data-stu-id="86ed0-106">educationAssignment: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86ed0-107">Это действие изменяет состояние назначения с исходного черновика на опубликованное.</span><span class="sxs-lookup"><span data-stu-id="86ed0-107">This action changes the state of an assignment from its original draft status to the published status.</span></span> <span data-ttu-id="86ed0-108">Только преподаватель в классе может совершать этот вызов.</span><span class="sxs-lookup"><span data-stu-id="86ed0-108">Only a teacher in the class can make this call.</span></span> <span data-ttu-id="86ed0-109">Если для назначения выбран статус черновика, студенты не увидят назначение и не будут иметь объектов отправки.</span><span class="sxs-lookup"><span data-stu-id="86ed0-109">When an assignment is in draft status, students will not see the assignment, nor will there be any submission objects.</span></span> <span data-ttu-id="86ed0-110">При вызове этого API создаются объекты отправки, а Назначение отображается в списке учащихся.</span><span class="sxs-lookup"><span data-stu-id="86ed0-110">When you call this API, submission objects are created and the assignment appears in the student's list.</span></span>

## <a name="permissions"></a><span data-ttu-id="86ed0-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86ed0-111">Permissions</span></span>
<span data-ttu-id="86ed0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86ed0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86ed0-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86ed0-114">Permission type</span></span>      | <span data-ttu-id="86ed0-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86ed0-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86ed0-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86ed0-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="86ed0-117">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86ed0-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="86ed0-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86ed0-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="86ed0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86ed0-119">Not supported.</span></span>  |
|<span data-ttu-id="86ed0-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86ed0-120">Application</span></span> | <span data-ttu-id="86ed0-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86ed0-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="86ed0-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86ed0-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="86ed0-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86ed0-123">Request headers</span></span>
| <span data-ttu-id="86ed0-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86ed0-124">Header</span></span>       | <span data-ttu-id="86ed0-125">Значение</span><span class="sxs-lookup"><span data-stu-id="86ed0-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="86ed0-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86ed0-126">Authorization</span></span>  | <span data-ttu-id="86ed0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86ed0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="86ed0-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86ed0-129">Request body</span></span>
<span data-ttu-id="86ed0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86ed0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86ed0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="86ed0-131">Response</span></span>
<span data-ttu-id="86ed0-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="86ed0-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86ed0-134">Пример</span><span class="sxs-lookup"><span data-stu-id="86ed0-134">Example</span></span>
<span data-ttu-id="86ed0-135">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="86ed0-135">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="86ed0-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="86ed0-136">Request</span></span>
<span data-ttu-id="86ed0-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86ed0-137">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/publish
```

##### <a name="response"></a><span data-ttu-id="86ed0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="86ed0-138">Response</span></span>
<span data-ttu-id="86ed0-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="86ed0-139">The following is an example of a response.</span></span> 

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
