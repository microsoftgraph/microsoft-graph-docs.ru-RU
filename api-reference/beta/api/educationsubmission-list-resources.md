---
title: Список ресурсов
description: Список ресурсов, связанных с этой отправки. Объект **submissionResource** — оболочкой вокруг объекта фактический ресурсов студент работает в. Если это скопированный из назначения во время процесса назначить программы-оболочки для также указатель ресурсов для назначения. Эти ресурсы, рабочую копию назначения. **SubmittedResources** представлены ресурсы, чтобы быть выражаемым числом отправленных официально.
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: d7476144159a8f2bd6c4600fe5a2eb80076bc7f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843983"
---
# <a name="list-resources"></a><span data-ttu-id="c3714-107">Список ресурсов</span><span class="sxs-lookup"><span data-stu-id="c3714-107">List resources</span></span>

> <span data-ttu-id="c3714-108">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c3714-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3714-109">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3714-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3714-110">Список ресурсов, связанных с этой отправки.</span><span class="sxs-lookup"><span data-stu-id="c3714-110">List the resources associated with this submission.</span></span> <span data-ttu-id="c3714-111">Объект **submissionResource** — оболочкой вокруг объекта фактический ресурсов студент работает в.</span><span class="sxs-lookup"><span data-stu-id="c3714-111">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="c3714-112">Если это скопированный из назначения во время процесса назначить программы-оболочки для также указатель ресурсов для назначения.</span><span class="sxs-lookup"><span data-stu-id="c3714-112">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="c3714-113">Эти ресурсы, рабочую копию назначения.</span><span class="sxs-lookup"><span data-stu-id="c3714-113">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="c3714-114">**SubmittedResources** представлены ресурсы, чтобы быть выражаемым числом отправленных официально.</span><span class="sxs-lookup"><span data-stu-id="c3714-114">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3714-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3714-115">Permissions</span></span>
<span data-ttu-id="c3714-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3714-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3714-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3714-118">Permission type</span></span>      | <span data-ttu-id="c3714-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3714-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3714-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3714-120">Delegated (work or school account)</span></span> |  <span data-ttu-id="c3714-121">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c3714-121">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="c3714-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3714-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3714-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3714-123">Not supported.</span></span>   |
|<span data-ttu-id="c3714-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3714-124">Application</span></span> | <span data-ttu-id="c3714-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3714-125">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c3714-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3714-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /educationClasses/assignments/{id}/submissions/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c3714-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c3714-127">Optional query parameters</span></span>
<span data-ttu-id="c3714-128">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c3714-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3714-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3714-129">Request headers</span></span>
| <span data-ttu-id="c3714-130">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3714-130">Header</span></span>       | <span data-ttu-id="c3714-131">Значение</span><span class="sxs-lookup"><span data-stu-id="c3714-131">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c3714-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3714-132">Authorization</span></span>  | <span data-ttu-id="c3714-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3714-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c3714-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c3714-135">Request body</span></span>
<span data-ttu-id="c3714-136">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3714-136">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c3714-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3714-137">Response</span></span>
<span data-ttu-id="c3714-138">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [educationSubmissionResource](../resources/educationsubmissionresource.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c3714-138">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3714-139">Пример</span><span class="sxs-lookup"><span data-stu-id="c3714-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3714-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3714-140">Request</span></span>
<span data-ttu-id="c3714-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3714-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments/<id>/submissions/<id>/resources
```
##### <a name="response"></a><span data-ttu-id="c3714-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3714-142">Response</span></span>
<span data-ttu-id="c3714-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c3714-143">The following is an example of the response.</span></span> 

><span data-ttu-id="c3714-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3714-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1045

{
  "value": [
    {
      "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
      "resource": {
          "@odata.type": "#microsoft.graph.educationLinkResource",
          "displayName": "Microsoft Homepage",
          "createdDateTime": "2017-10-21T07:52:45.5675913Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "link": "https://www.microsoft.com"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
