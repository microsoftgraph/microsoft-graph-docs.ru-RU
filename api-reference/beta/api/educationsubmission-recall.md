---
title: 'educationSubmission: отзыв'
description: 'Указывает, что студенту требуется выполнить отправку. Это действие можно выполнить только студентом. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 847dfc4d3e868243ea8120fee927fe1397a4826c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322954"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="25d55-104">educationSubmission: отзыв</span><span class="sxs-lookup"><span data-stu-id="25d55-104">educationSubmission: recall</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25d55-105">Указывает, что студенту требуется выполнить отправку.</span><span class="sxs-lookup"><span data-stu-id="25d55-105">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="25d55-106">Это действие можно выполнить только студентом.</span><span class="sxs-lookup"><span data-stu-id="25d55-106">This action can only be done by a student.</span></span> <span data-ttu-id="25d55-107">Он изменит состояние отправки с "Отправлено" обратно на "работает".</span><span class="sxs-lookup"><span data-stu-id="25d55-107">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="25d55-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25d55-108">Permissions</span></span>
<span data-ttu-id="25d55-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25d55-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25d55-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25d55-111">Permission type</span></span>      | <span data-ttu-id="25d55-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25d55-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25d55-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25d55-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="25d55-114">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25d55-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="25d55-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25d55-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="25d55-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="25d55-116">Not supported</span></span>  |
|<span data-ttu-id="25d55-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25d55-117">Application</span></span> |<span data-ttu-id="25d55-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25d55-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="25d55-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25d55-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="25d55-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25d55-120">Request headers</span></span>
| <span data-ttu-id="25d55-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25d55-121">Header</span></span>       | <span data-ttu-id="25d55-122">Значение</span><span class="sxs-lookup"><span data-stu-id="25d55-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="25d55-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25d55-123">Authorization</span></span>  | <span data-ttu-id="25d55-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25d55-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="25d55-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25d55-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="25d55-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="25d55-127">Response</span></span>
<span data-ttu-id="25d55-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="25d55-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25d55-130">Пример</span><span class="sxs-lookup"><span data-stu-id="25d55-130">Example</span></span>
<span data-ttu-id="25d55-131">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="25d55-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="25d55-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="25d55-132">Request</span></span>
<span data-ttu-id="25d55-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25d55-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="25d55-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="25d55-134">Response</span></span>
<span data-ttu-id="25d55-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="25d55-135">The following is an example of the response.</span></span>

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
  "description": "educationSubmission: recall",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
