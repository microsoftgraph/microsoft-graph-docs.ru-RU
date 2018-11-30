---
title: Получение educationSubmissionResource
description: " Список ресурсов и должны считаться студент рабочего процесса. Этот ресурс оболочку с возможные указатель обратно в назначения ресурсов, если он был скопирован из назначения."
ms.openlocfilehash: 1bba0b8b4e89b0f3bc564f48187cfe46fc49cf46
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074974"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="64cc4-104">Получение educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="64cc4-104">Get educationSubmissionResource</span></span>

> <span data-ttu-id="64cc4-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="64cc4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64cc4-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64cc4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="64cc4-107">Получает свойства определенного ресурса, связанного с подачи.</span><span class="sxs-lookup"><span data-stu-id="64cc4-107">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="64cc4-108">Этот ресурс находится в списке ресурсов «рабочий» и должны считаться рабочего процесса студента.</span><span class="sxs-lookup"><span data-stu-id="64cc4-108">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="64cc4-109">Этот ресурс оболочку с возможные указатель обратно в назначения ресурсов, если он был скопирован из назначения.</span><span class="sxs-lookup"><span data-stu-id="64cc4-109">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="64cc4-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64cc4-110">Permissions</span></span>
<span data-ttu-id="64cc4-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64cc4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64cc4-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64cc4-113">Permission type</span></span>      | <span data-ttu-id="64cc4-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64cc4-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64cc4-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64cc4-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="64cc4-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64cc4-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="64cc4-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64cc4-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="64cc4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64cc4-118">Not supported.</span></span>  |
|<span data-ttu-id="64cc4-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64cc4-119">Application</span></span> | <span data-ttu-id="64cc4-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64cc4-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="64cc4-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64cc4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="64cc4-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="64cc4-122">Optional query parameters</span></span>
<span data-ttu-id="64cc4-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="64cc4-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64cc4-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64cc4-124">Request headers</span></span>
| <span data-ttu-id="64cc4-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64cc4-125">Header</span></span>       | <span data-ttu-id="64cc4-126">Значение</span><span class="sxs-lookup"><span data-stu-id="64cc4-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="64cc4-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64cc4-127">Authorization</span></span>  | <span data-ttu-id="64cc4-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64cc4-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="64cc4-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64cc4-130">Request body</span></span>
<span data-ttu-id="64cc4-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64cc4-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="64cc4-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="64cc4-132">Response</span></span>
<span data-ttu-id="64cc4-133">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [educationSubmissionResource](../resources/educationsubmissionresource.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="64cc4-133">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="64cc4-134">Пример</span><span class="sxs-lookup"><span data-stu-id="64cc4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64cc4-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="64cc4-135">Request</span></span>
<span data-ttu-id="64cc4-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64cc4-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmissionresource"
}-->
```http 
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="64cc4-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="64cc4-137">Response</span></span>
<span data-ttu-id="64cc4-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="64cc4-138">The following is an example of the response.</span></span> 

><span data-ttu-id="64cc4-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64cc4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1152

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
  "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
  "resource": {
      "@odata.type": "#microsoft.graph.educationWordResource",
      "displayName": "Report.docx",
      "createdDateTime": "2017-10-21T07:52:53.9863696Z",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2017-10-21T07:52:53.9863696Z",
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
