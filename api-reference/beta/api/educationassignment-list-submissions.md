---
title: Отправка сообщений о списка
description: Список всех отправленных данных, связанных с данного назначения. Преподаватель можно получить всех отправляемых во время студента можно получить только отправленные данные, связанные с ними.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 47088cb7a4290827ce75e35d3ac705b31addefac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510640"
---
# <a name="list-submissions"></a><span data-ttu-id="ebed1-104">Отправка сообщений о списка</span><span class="sxs-lookup"><span data-stu-id="ebed1-104">List submissions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebed1-105">Список всех отправленных данных, связанных с данного назначения.</span><span class="sxs-lookup"><span data-stu-id="ebed1-105">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="ebed1-106">Преподаватель можно получить всех отправляемых во время студента можно получить только отправленные данные, связанные с ними.</span><span class="sxs-lookup"><span data-stu-id="ebed1-106">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebed1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebed1-107">Permissions</span></span>
<span data-ttu-id="ebed1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebed1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebed1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebed1-110">Permission type</span></span>      | <span data-ttu-id="ebed1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebed1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebed1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebed1-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="ebed1-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ebed1-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="ebed1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebed1-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ebed1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebed1-115">Not supported.</span></span>  |
|<span data-ttu-id="ebed1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebed1-116">Application</span></span> | <span data-ttu-id="ebed1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebed1-117">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ebed1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebed1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ebed1-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ebed1-119">Optional query parameters</span></span>
<span data-ttu-id="ebed1-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ebed1-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ebed1-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebed1-121">Request headers</span></span>
| <span data-ttu-id="ebed1-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ebed1-122">Header</span></span>       | <span data-ttu-id="ebed1-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ebed1-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ebed1-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ebed1-124">Authorization</span></span>  | <span data-ttu-id="ebed1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebed1-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ebed1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ebed1-127">Request body</span></span>
<span data-ttu-id="ebed1-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ebed1-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ebed1-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="ebed1-129">Response</span></span>
<span data-ttu-id="ebed1-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [educationSubmission](../resources/educationsubmission.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ebed1-130">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ebed1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ebed1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebed1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebed1-132">Request</span></span>
<span data-ttu-id="ebed1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ebed1-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="ebed1-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ebed1-134">Response</span></span>
<span data-ttu-id="ebed1-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ebed1-135">The following is an example of the response.</span></span> 

><span data-ttu-id="ebed1-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ebed1-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ebed1-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ebed1-137">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
  "value": [
    {
      "feedback": {
        "text": {
          "content": "Good work!",
          "contentType": "Text"
        },
        "feedbackDateTime": "2014-01-01T00:00:00Z",
        "feedbackBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
          "@odata.type": "microsoft.graph.identitySet"
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
        "userId": "13015",
        "@Odata.type":"microsoft.graph.educationSubmissionRecipient"
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List submissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-list-submissions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
