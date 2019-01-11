---
title: Список submittedResources
description: Список ресурсов, поданных официально для ранжирования. Учебы, ответственных за подачи не может изменить отправляемого списка без повторной отправки назначения. Это является оболочкой реальных ресурсов и может содержать указатель фактический назначения ресурса, если этот ресурс, скопированный из назначения.
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: da036713e6683aaef6576145dfe32b3b6eeaf11e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824145"
---
# <a name="list-submittedresources"></a><span data-ttu-id="4fbbb-105">Список submittedResources</span><span class="sxs-lookup"><span data-stu-id="4fbbb-105">List submittedResources</span></span>

> <span data-ttu-id="4fbbb-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4fbbb-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4fbbb-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fbbb-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4fbbb-108">Список ресурсов, поданных официально для ранжирования.</span><span class="sxs-lookup"><span data-stu-id="4fbbb-108">List the resources that have officially been submitted for grading.</span></span> <span data-ttu-id="4fbbb-109">Учебы, ответственных за подачи не может изменить отправляемого списка без повторной отправки назначения.</span><span class="sxs-lookup"><span data-stu-id="4fbbb-109">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="4fbbb-110">Это является оболочкой реальных ресурсов и может содержать указатель фактический назначения ресурса, если этот ресурс, скопированный из назначения.</span><span class="sxs-lookup"><span data-stu-id="4fbbb-110">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="4fbbb-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4fbbb-111">Permissions</span></span>
<span data-ttu-id="4fbbb-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fbbb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fbbb-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fbbb-114">Permission type</span></span>      | <span data-ttu-id="4fbbb-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fbbb-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4fbbb-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fbbb-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="4fbbb-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4fbbb-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="4fbbb-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fbbb-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4fbbb-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fbbb-119">Not supported.</span></span>  |
|<span data-ttu-id="4fbbb-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fbbb-120">Application</span></span> | <span data-ttu-id="4fbbb-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fbbb-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4fbbb-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fbbb-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4fbbb-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4fbbb-123">Optional query parameters</span></span>
<span data-ttu-id="4fbbb-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4fbbb-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4fbbb-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4fbbb-125">Request headers</span></span>
| <span data-ttu-id="4fbbb-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4fbbb-126">Header</span></span>       | <span data-ttu-id="4fbbb-127">Значение</span><span class="sxs-lookup"><span data-stu-id="4fbbb-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4fbbb-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4fbbb-128">Authorization</span></span>  | <span data-ttu-id="4fbbb-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fbbb-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4fbbb-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4fbbb-131">Request body</span></span>
<span data-ttu-id="4fbbb-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4fbbb-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4fbbb-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="4fbbb-133">Response</span></span>
<span data-ttu-id="4fbbb-134">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [educationSubmissionResource](../resources/educationsubmissionresource.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4fbbb-134">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4fbbb-135">Пример</span><span class="sxs-lookup"><span data-stu-id="4fbbb-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4fbbb-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fbbb-136">Request</span></span>
<span data-ttu-id="4fbbb-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fbbb-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources
```
##### <a name="response"></a><span data-ttu-id="4fbbb-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="4fbbb-138">Response</span></span>
<span data-ttu-id="4fbbb-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4fbbb-139">The following is an example of the response.</span></span> 

><span data-ttu-id="4fbbb-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4fbbb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource",
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
        "link": "https://www.microsoft.com
        },
        "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource" 
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List submittedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
