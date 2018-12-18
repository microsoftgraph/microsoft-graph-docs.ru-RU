---
title: Получение educationSubmission
description: 'Получение определенного отправки. Объект отправки представляет учащихся трудозатраты для назначения. Ресурсы, связанные с представляют отправки этой функции. Студент подачи присваивается можно просмотреть и изменить подачи. Преподаватель имеет полный доступ для всех отправляемых. '
author: dipakboyed
ms.openlocfilehash: 39e3591c0236d7a6fbc4896d4009fe5a00157d9d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353083"
---
# <a name="get-educationsubmission"></a><span data-ttu-id="2f632-107">Получение educationSubmission</span><span class="sxs-lookup"><span data-stu-id="2f632-107">Get educationSubmission</span></span>

> <span data-ttu-id="2f632-108">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2f632-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f632-109">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f632-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2f632-110">Получение определенного отправки.</span><span class="sxs-lookup"><span data-stu-id="2f632-110">Retrieve a particular submission.</span></span> <span data-ttu-id="2f632-111">Объект отправки представляет учащихся трудозатраты для назначения.</span><span class="sxs-lookup"><span data-stu-id="2f632-111">A submission object represents a student's work for an assignment.</span></span> <span data-ttu-id="2f632-112">Ресурсы, связанные с представляют отправки этой функции.</span><span class="sxs-lookup"><span data-stu-id="2f632-112">Resources associated with the submission represent this work.</span></span> <span data-ttu-id="2f632-113">Студент подачи присваивается можно просмотреть и изменить подачи.</span><span class="sxs-lookup"><span data-stu-id="2f632-113">Only the student the submission is assigned to can see and modify the submission.</span></span> <span data-ttu-id="2f632-114">Преподаватель имеет полный доступ для всех отправляемых.</span><span class="sxs-lookup"><span data-stu-id="2f632-114">A teacher has full access to all submissions.</span></span> 

<span data-ttu-id="2f632-115">Марки и свои отзывы и предложения из учитель также являются частью этого объекта.</span><span class="sxs-lookup"><span data-stu-id="2f632-115">The grade and feedback from a teacher are also part of this object.</span></span> <span data-ttu-id="2f632-116">Только учителя можно добавлять или изменять оценки и отзывы.</span><span class="sxs-lookup"><span data-stu-id="2f632-116">Only teachers can add or change grades and feedback.</span></span> <span data-ttu-id="2f632-117">Студентов не будут отображаться марки или свои отзывы и предложения, пока не было освобождено назначения.</span><span class="sxs-lookup"><span data-stu-id="2f632-117">Students will not see the grade or feedback until the assignment has been released.</span></span> <span data-ttu-id="2f632-118">Основные разрешения не следует включать оценку и свои отзывы и предложения, но включают все остальное.</span><span class="sxs-lookup"><span data-stu-id="2f632-118">The Basic permissions do not include grade and feedback but do include everything else.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f632-119">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f632-119">Permissions</span></span>
<span data-ttu-id="2f632-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f632-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f632-122">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f632-122">Permission type</span></span>      | <span data-ttu-id="2f632-123">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f632-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f632-124">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f632-124">Delegated (work or school account)</span></span> |  <span data-ttu-id="2f632-125">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f632-125">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="2f632-126">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f632-126">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2f632-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f632-127">Not supported.</span></span>  |
|<span data-ttu-id="2f632-128">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f632-128">Application</span></span> | <span data-ttu-id="2f632-129">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f632-129">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2f632-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f632-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2f632-131">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2f632-131">Optional query parameters</span></span>
<span data-ttu-id="2f632-132">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2f632-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f632-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f632-133">Request headers</span></span>
| <span data-ttu-id="2f632-134">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f632-134">Header</span></span>       | <span data-ttu-id="2f632-135">Значение</span><span class="sxs-lookup"><span data-stu-id="2f632-135">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f632-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f632-136">Authorization</span></span>  | <span data-ttu-id="2f632-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f632-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f632-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f632-139">Request body</span></span>
<span data-ttu-id="2f632-140">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f632-140">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2f632-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f632-141">Response</span></span>
<span data-ttu-id="2f632-142">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [educationSubmission](../resources/educationsubmission.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2f632-142">If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2f632-143">Пример</span><span class="sxs-lookup"><span data-stu-id="2f632-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f632-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f632-144">Request</span></span>
<span data-ttu-id="2f632-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f632-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmission"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11010/assignments/19002/submissions/33223
```
##### <a name="response"></a><span data-ttu-id="2f632-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f632-146">Response</span></span>
<span data-ttu-id="2f632-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2f632-147">The following is an example of the response.</span></span> 

><span data-ttu-id="2f632-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f632-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->