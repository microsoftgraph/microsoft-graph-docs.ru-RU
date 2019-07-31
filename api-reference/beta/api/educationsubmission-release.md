---
title: 'educationSubmission: Release'
description: " Указывает, что выполняется ступенчатое выполнение. Это действие может выполнить только преподаватель."
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ddf437c60ae4ca56a800bd82b081b149a686eabe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955082"
---
# <a name="educationsubmission-release"></a><span data-ttu-id="9db03-104">educationSubmission: Release</span><span class="sxs-lookup"><span data-stu-id="9db03-104">educationSubmission: release</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9db03-105">Это действие делает оценку и обратную связь, связанную с этой отправкой, доступной студенту.</span><span class="sxs-lookup"><span data-stu-id="9db03-105">This action makes the grade and feedback associated with this submission available to the student.</span></span> <span data-ttu-id="9db03-106">Это приведет к изменению состояния отправки с "Отправлено" на "выпущено" и указывает на то, что выполняется ступенчатое выполнение.</span><span class="sxs-lookup"><span data-stu-id="9db03-106">This will change the status of the submission from "submitted" to "released" and indicates that grading is done.</span></span> <span data-ttu-id="9db03-107">Это действие может выполнить только преподаватель.</span><span class="sxs-lookup"><span data-stu-id="9db03-107">This action can only be done by the teacher.</span></span>

## <a name="permissions"></a><span data-ttu-id="9db03-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9db03-108">Permissions</span></span>
<span data-ttu-id="9db03-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9db03-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9db03-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9db03-111">Permission type</span></span>      | <span data-ttu-id="9db03-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9db03-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9db03-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9db03-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="9db03-114">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9db03-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="9db03-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9db03-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9db03-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9db03-116">Not supported.</span></span>  |
|<span data-ttu-id="9db03-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9db03-117">Application</span></span> | <span data-ttu-id="9db03-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9db03-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9db03-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9db03-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/release

```
## <a name="request-headers"></a><span data-ttu-id="9db03-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9db03-120">Request headers</span></span>
| <span data-ttu-id="9db03-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9db03-121">Header</span></span>       | <span data-ttu-id="9db03-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9db03-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9db03-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9db03-123">Authorization</span></span>  | <span data-ttu-id="9db03-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9db03-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9db03-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9db03-126">Request body</span></span>
<span data-ttu-id="9db03-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9db03-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9db03-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="9db03-128">Response</span></span>
<span data-ttu-id="9db03-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9db03-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9db03-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9db03-131">Example</span></span>
<span data-ttu-id="9db03-132">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="9db03-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9db03-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9db03-133">Request</span></span>
<span data-ttu-id="9db03-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9db03-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_release"
}-->

```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/release
```

##### <a name="response"></a><span data-ttu-id="9db03-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9db03-135">Response</span></span>
<span data-ttu-id="9db03-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9db03-136">The following is an example of the response.</span></span>

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
