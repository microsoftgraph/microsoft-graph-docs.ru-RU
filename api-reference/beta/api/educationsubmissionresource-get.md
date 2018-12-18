---
title: Получение educationSubmissionResource
description: Получает свойства определенного ресурса, связанного с подачи. Этот ресурс находится в списке ресурсов «рабочий» и должны считаться рабочего процесса студента. Этот ресурс оболочку с возможные указатель обратно в назначения ресурсов, если он был скопирован из назначения.
author: dipakboyed
ms.openlocfilehash: d7c1e6fcbe97a9a0a4c1735e37798097f2605b30
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361917"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="30628-105">Получение educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="30628-105">Get educationSubmissionResource</span></span>

> <span data-ttu-id="30628-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="30628-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30628-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30628-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="30628-108">Получает свойства определенного ресурса, связанного с подачи.</span><span class="sxs-lookup"><span data-stu-id="30628-108">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="30628-109">Этот ресурс находится в списке ресурсов «рабочий» и должны считаться рабочего процесса студента.</span><span class="sxs-lookup"><span data-stu-id="30628-109">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="30628-110">Этот ресурс оболочку с возможные указатель обратно в назначения ресурсов, если он был скопирован из назначения.</span><span class="sxs-lookup"><span data-stu-id="30628-110">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="30628-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30628-111">Permissions</span></span>
<span data-ttu-id="30628-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30628-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30628-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30628-114">Permission type</span></span>      | <span data-ttu-id="30628-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30628-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30628-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30628-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="30628-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30628-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="30628-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30628-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="30628-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30628-119">Not supported.</span></span>  |
|<span data-ttu-id="30628-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30628-120">Application</span></span> | <span data-ttu-id="30628-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30628-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="30628-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30628-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="30628-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="30628-123">Optional query parameters</span></span>
<span data-ttu-id="30628-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="30628-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="30628-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30628-125">Request headers</span></span>
| <span data-ttu-id="30628-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30628-126">Header</span></span>       | <span data-ttu-id="30628-127">Значение</span><span class="sxs-lookup"><span data-stu-id="30628-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="30628-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30628-128">Authorization</span></span>  | <span data-ttu-id="30628-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30628-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="30628-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30628-131">Request body</span></span>
<span data-ttu-id="30628-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30628-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="30628-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="30628-133">Response</span></span>
<span data-ttu-id="30628-134">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [educationSubmissionResource](../resources/educationsubmissionresource.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="30628-134">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="30628-135">Пример</span><span class="sxs-lookup"><span data-stu-id="30628-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30628-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="30628-136">Request</span></span>
<span data-ttu-id="30628-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30628-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmissionresource"
}-->
```http 
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="30628-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="30628-138">Response</span></span>
<span data-ttu-id="30628-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="30628-139">The following is an example of the response.</span></span> 

><span data-ttu-id="30628-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30628-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
