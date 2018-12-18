---
title: Отправка сообщений о списка
description: Список всех отправленных данных, связанных с данного назначения. Преподаватель можно получить всех отправляемых во время студента можно получить только отправленные данные, связанные с ними.
author: dipakboyed
ms.openlocfilehash: ac7bd47b4cbc4549f38239c4a68504bd20b3a2e8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308430"
---
# <a name="list-submissions"></a><span data-ttu-id="b85f8-104">Отправка сообщений о списка</span><span class="sxs-lookup"><span data-stu-id="b85f8-104">List submissions</span></span>

> <span data-ttu-id="b85f8-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b85f8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b85f8-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b85f8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b85f8-107">Список всех отправленных данных, связанных с данного назначения.</span><span class="sxs-lookup"><span data-stu-id="b85f8-107">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="b85f8-108">Преподаватель можно получить всех отправляемых во время студента можно получить только отправленные данные, связанные с ними.</span><span class="sxs-lookup"><span data-stu-id="b85f8-108">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="b85f8-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b85f8-109">Permissions</span></span>
<span data-ttu-id="b85f8-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b85f8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b85f8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b85f8-112">Permission type</span></span>      | <span data-ttu-id="b85f8-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b85f8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b85f8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b85f8-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="b85f8-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b85f8-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="b85f8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b85f8-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b85f8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b85f8-117">Not supported.</span></span>  |
|<span data-ttu-id="b85f8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b85f8-118">Application</span></span> | <span data-ttu-id="b85f8-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b85f8-119">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b85f8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b85f8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b85f8-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b85f8-121">Optional query parameters</span></span>
<span data-ttu-id="b85f8-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b85f8-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b85f8-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b85f8-123">Request headers</span></span>
| <span data-ttu-id="b85f8-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b85f8-124">Header</span></span>       | <span data-ttu-id="b85f8-125">Значение</span><span class="sxs-lookup"><span data-stu-id="b85f8-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b85f8-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b85f8-126">Authorization</span></span>  | <span data-ttu-id="b85f8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b85f8-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b85f8-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b85f8-129">Request body</span></span>
<span data-ttu-id="b85f8-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b85f8-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b85f8-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="b85f8-131">Response</span></span>
<span data-ttu-id="b85f8-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [educationSubmission](../resources/educationsubmission.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b85f8-132">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b85f8-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b85f8-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b85f8-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b85f8-134">Request</span></span>
<span data-ttu-id="b85f8-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b85f8-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="b85f8-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="b85f8-136">Response</span></span>
<span data-ttu-id="b85f8-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b85f8-137">The following is an example of the response.</span></span> 

><span data-ttu-id="b85f8-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b85f8-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b85f8-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b85f8-139">All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List submissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->