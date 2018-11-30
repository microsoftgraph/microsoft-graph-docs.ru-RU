---
title: Список educationAssignmentResources
description: Получите все ресурсы, связанные с этим назначением.
ms.openlocfilehash: 2092b7a98794bc8eaeac7e65eea5dced8ffa00d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077558"
---
# <a name="list-educationassignmentresources"></a><span data-ttu-id="e2e78-103">Список educationAssignmentResources</span><span class="sxs-lookup"><span data-stu-id="e2e78-103">List educationAssignmentResources</span></span>

> <span data-ttu-id="e2e78-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e2e78-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2e78-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2e78-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2e78-106">Получите все ресурсы, связанные с этим назначением.</span><span class="sxs-lookup"><span data-stu-id="e2e78-106">Get all the resources associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2e78-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2e78-107">Permissions</span></span>
<span data-ttu-id="e2e78-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2e78-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2e78-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2e78-110">Permission type</span></span>      | <span data-ttu-id="e2e78-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2e78-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2e78-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2e78-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="e2e78-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2e78-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e2e78-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2e78-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e2e78-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2e78-115">Not supported.</span></span>  |
|<span data-ttu-id="e2e78-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2e78-116">Application</span></span> | <span data-ttu-id="e2e78-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2e78-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e2e78-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2e78-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e2e78-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e2e78-119">Optional query parameters</span></span>
<span data-ttu-id="e2e78-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e2e78-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2e78-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2e78-121">Request headers</span></span>
| <span data-ttu-id="e2e78-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2e78-122">Header</span></span>       | <span data-ttu-id="e2e78-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e2e78-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e2e78-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e2e78-124">Authorization</span></span>  | <span data-ttu-id="e2e78-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2e78-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e2e78-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2e78-127">Request body</span></span>
<span data-ttu-id="e2e78-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2e78-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e2e78-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2e78-129">Response</span></span>
<span data-ttu-id="e2e78-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [educationAssignmentResource](../resources/educationassignmentresource.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e2e78-130">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e2e78-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e2e78-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2e78-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2e78-132">Request</span></span>
<span data-ttu-id="e2e78-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2e78-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/resources
```
##### <a name="response"></a><span data-ttu-id="e2e78-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e2e78-134">Response</span></span>
<span data-ttu-id="e2e78-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e2e78-135">The following is an example of the response.</span></span> 

><span data-ttu-id="e2e78-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2e78-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1011

{
  "value": [
    {
      "distributeForStudentWork": false,
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
      },
      "id": "850f51b7-1df9-4ec0-bd62-64a0214b9cbf"
    },
    {
      "distributeForStudentWork": true,
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
      },
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024"
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
