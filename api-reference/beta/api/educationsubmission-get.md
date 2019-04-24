---
title: Получение educationSubmission
description: 'Получение определенной отправки. Объект отправки представляет работу учащегося для назначения. Ресурсы, связанные с отправкой, представляют эту работу. Только студент, которому назначена отправка, может просматривать и изменять отправку. Преподаватель имеет полный доступ ко всем отправку. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d0542bec537b8317a46e98c215768f5228f9a07c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457653"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="d07fd-107">Получение educationSubmission</span><span class="sxs-lookup"><span data-stu-id="d07fd-107">Get educationSubmission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d07fd-108">Получение определенной отправки.</span><span class="sxs-lookup"><span data-stu-id="d07fd-108">Retrieve a particular submission.</span></span> <span data-ttu-id="d07fd-109">Объект отправки представляет работу учащегося для назначения.</span><span class="sxs-lookup"><span data-stu-id="d07fd-109">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="d07fd-110">Ресурсы, связанные с отправкой, представляют эту работу.</span><span class="sxs-lookup"><span data-stu-id="d07fd-110">Resources associated with the submission represent this work.</span></span> <span data-ttu-id="d07fd-111">Только студент, которому назначена отправка, может просматривать и изменять отправку.</span><span class="sxs-lookup"><span data-stu-id="d07fd-111">Only the student the submission is assigned to can see and modify the submission.</span></span> <span data-ttu-id="d07fd-112">Преподаватель имеет полный доступ ко всем отправку.</span><span class="sxs-lookup"><span data-stu-id="d07fd-112">A teacher has full access to all submissions.</span></span> 

<span data-ttu-id="d07fd-113">Оценка и обратная связь с преподавателем также являются частью этого объекта.</span><span class="sxs-lookup"><span data-stu-id="d07fd-113">The grade and feedback from a teacher are also part of this object.</span></span> <span data-ttu-id="d07fd-114">Только преподаватели могут добавлять или изменять оценки и отзывы.</span><span class="sxs-lookup"><span data-stu-id="d07fd-114">Only teachers can add or change grades and feedback.</span></span> <span data-ttu-id="d07fd-115">Студенты не увидят оценку или обратную связь, пока не будет выпущено назначение.</span><span class="sxs-lookup"><span data-stu-id="d07fd-115">Students will not see the grade or feedback until the assignment has been released.</span></span> <span data-ttu-id="d07fd-116">Основные разрешения не включают оценку и обратную связь, но включают все остальные.</span><span class="sxs-lookup"><span data-stu-id="d07fd-116">The Basic permissions do not include grade and feedback but do include everything else.</span></span>

## <a name="permissions"></a><span data-ttu-id="d07fd-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d07fd-117">Permissions</span></span>
<span data-ttu-id="d07fd-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d07fd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d07fd-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d07fd-120">Permission type</span></span>      | <span data-ttu-id="d07fd-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d07fd-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d07fd-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d07fd-122">Delegated (work or school account)</span></span> |  <span data-ttu-id="d07fd-123">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d07fd-123">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="d07fd-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d07fd-124">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d07fd-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d07fd-125">Not supported.</span></span>  |
|<span data-ttu-id="d07fd-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d07fd-126">Application</span></span> | <span data-ttu-id="d07fd-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d07fd-127">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d07fd-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d07fd-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d07fd-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d07fd-129">Optional query parameters</span></span>
<span data-ttu-id="d07fd-130">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d07fd-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d07fd-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d07fd-131">Request headers</span></span>
| <span data-ttu-id="d07fd-132">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d07fd-132">Header</span></span>       | <span data-ttu-id="d07fd-133">Значение</span><span class="sxs-lookup"><span data-stu-id="d07fd-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d07fd-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d07fd-134">Authorization</span></span>  | <span data-ttu-id="d07fd-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d07fd-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d07fd-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d07fd-137">Request body</span></span>
<span data-ttu-id="d07fd-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d07fd-138">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d07fd-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="d07fd-139">Response</span></span>
<span data-ttu-id="d07fd-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [educationSubmission](../resources/educationsubmission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d07fd-140">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d07fd-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d07fd-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d07fd-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d07fd-142">Request</span></span>
<span data-ttu-id="d07fd-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d07fd-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmission"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
##### <a name="response"></a><span data-ttu-id="d07fd-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d07fd-144">Response</span></span>
<span data-ttu-id="d07fd-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d07fd-145">The following is an example of the response.</span></span> 

><span data-ttu-id="d07fd-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d07fd-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 712

{
    "feedback": {
      text: {
        "content": "Good work!",
        "contentType": "Text"
      },
      feedbackDateTime: "2014-01-01T00:00:00Z",
      feedbackBy: {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012"
        }
      },
      "@odata.type": "microsoft.graph.educationFeedback"
      },
      "grade": {
         "gradedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
        "gradedDateTime": "2014-01-01T00:00:00Z"
      },
      "id": "33223",
      "recipient": {
        "userId": "13015"
      },
      "releasedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "releasedDateTime": "2014-01-01T00:00:00Z",
      "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "status": "working",
      "submittedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "submittedDateTime": "2014-01-01T00:00:00Z"
    }
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
