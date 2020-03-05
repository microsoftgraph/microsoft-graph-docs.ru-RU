---
title: 'educationSubmission: Release'
description: " Указывает, что выполняется ступенчатое выполнение. Это действие может выполнить только преподаватель."
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ac1678381a89402d9005c6bd198d2cee3f3178db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424857"
---
# <a name="educationsubmission-release"></a><span data-ttu-id="71fa3-104">educationSubmission: Release</span><span class="sxs-lookup"><span data-stu-id="71fa3-104">educationSubmission: release</span></span>

<span data-ttu-id="71fa3-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="71fa3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71fa3-106">Это действие делает [едукатионауткоме](../resources/educationoutcome.md) , включая любые оценки или отзывы, связанные с этой отправкой, доступными для учащегося.</span><span class="sxs-lookup"><span data-stu-id="71fa3-106">This action makes the [educationOutcome](../resources/educationoutcome.md) including any grades or feedback associated with this submission available to the student.</span></span> <span data-ttu-id="71fa3-107">Это приведет к изменению состояния отправки с "Отправлено" на "выпущено" и указывает на то, что выполняется ступенчатое выполнение.</span><span class="sxs-lookup"><span data-stu-id="71fa3-107">This will change the status of the submission from "submitted" to "released" and indicates that grading is done.</span></span> <span data-ttu-id="71fa3-108">Это действие может выполнить только преподаватель.</span><span class="sxs-lookup"><span data-stu-id="71fa3-108">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="71fa3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71fa3-109">Permissions</span></span>
<span data-ttu-id="71fa3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71fa3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71fa3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71fa3-112">Permission type</span></span>      | <span data-ttu-id="71fa3-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71fa3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71fa3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71fa3-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="71fa3-115">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71fa3-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="71fa3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71fa3-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="71fa3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71fa3-117">Not supported.</span></span>  |
|<span data-ttu-id="71fa3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71fa3-118">Application</span></span> | <span data-ttu-id="71fa3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71fa3-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="71fa3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71fa3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/release

```
## <a name="request-headers"></a><span data-ttu-id="71fa3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71fa3-121">Request headers</span></span>
| <span data-ttu-id="71fa3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71fa3-122">Header</span></span>       | <span data-ttu-id="71fa3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="71fa3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="71fa3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71fa3-124">Authorization</span></span>  | <span data-ttu-id="71fa3-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71fa3-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71fa3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71fa3-127">Request body</span></span>
<span data-ttu-id="71fa3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71fa3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71fa3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="71fa3-129">Response</span></span>
<span data-ttu-id="71fa3-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="71fa3-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71fa3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="71fa3-132">Example</span></span>
<span data-ttu-id="71fa3-133">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="71fa3-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="71fa3-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="71fa3-134">Request</span></span>
<span data-ttu-id="71fa3-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71fa3-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_release"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/release
```

##### <a name="response"></a><span data-ttu-id="71fa3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="71fa3-136">Response</span></span>
<span data-ttu-id="71fa3-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="71fa3-137">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: release",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
