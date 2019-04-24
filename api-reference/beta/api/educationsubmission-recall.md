---
title: 'educationSubmission: отзыв'
description: 'Указывает, что студенту требуется выполнить отправку. Это действие можно выполнить только студентом. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0be94d2888223ca31e37b71e490c4a9fdc28b7d0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457632"
---
# <a name="educationsubmission-recall"></a><span data-ttu-id="822c6-104">educationSubmission: отзыв</span><span class="sxs-lookup"><span data-stu-id="822c6-104">educationSubmission: recall</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="822c6-105">Указывает, что студенту требуется выполнить отправку.</span><span class="sxs-lookup"><span data-stu-id="822c6-105">Indicates that a student wants to take back a submission.</span></span> <span data-ttu-id="822c6-106">Это действие можно выполнить только студентом.</span><span class="sxs-lookup"><span data-stu-id="822c6-106">This action can only be done by a student.</span></span> <span data-ttu-id="822c6-107">Он изменит состояние отправки с "Отправлено" обратно на "работает".</span><span class="sxs-lookup"><span data-stu-id="822c6-107">It will change the status of the submission from "submitted" back to "working".</span></span>

## <a name="permissions"></a><span data-ttu-id="822c6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="822c6-108">Permissions</span></span>
<span data-ttu-id="822c6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="822c6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="822c6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="822c6-111">Permission type</span></span>      | <span data-ttu-id="822c6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="822c6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="822c6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="822c6-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="822c6-114">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="822c6-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="822c6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="822c6-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="822c6-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="822c6-116">Not supported</span></span>  |
|<span data-ttu-id="822c6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="822c6-117">Application</span></span> |<span data-ttu-id="822c6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="822c6-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="822c6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="822c6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/<id>/assignments/{id}/submissions/{id}/recall

```
## <a name="request-headers"></a><span data-ttu-id="822c6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="822c6-120">Request headers</span></span>
| <span data-ttu-id="822c6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="822c6-121">Header</span></span>       | <span data-ttu-id="822c6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="822c6-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="822c6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="822c6-123">Authorization</span></span>  | <span data-ttu-id="822c6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="822c6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="822c6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="822c6-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="822c6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="822c6-127">Response</span></span>
<span data-ttu-id="822c6-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="822c6-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="822c6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="822c6-130">Example</span></span>
<span data-ttu-id="822c6-131">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="822c6-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="822c6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="822c6-132">Request</span></span>
<span data-ttu-id="822c6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="822c6-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationsubmission_recall"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/recall
```

##### <a name="response"></a><span data-ttu-id="822c6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="822c6-134">Response</span></span>
<span data-ttu-id="822c6-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="822c6-135">The following is an example of the response.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-recall.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
