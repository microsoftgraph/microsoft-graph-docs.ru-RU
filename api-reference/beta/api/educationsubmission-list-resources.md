---
title: Список ресурсов
description: ПереЧислите ресурсы, связанные с этой отправкой. Объект **субмиссионресаурце** является оболочкой для фактического объекта ресурса, над которым работает учащийся. Кроме того, обертка содержит указатель на ресурсы назначения, который был скопирован из назначения во время процесса Assign. Эти ресурсы являются рабочей копией назначения. **Субмиттедресаурцес** — это ресурсы, которые официально передаются на производительность.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b9069cb6ec20f65b82cacca8f862a05ff0af7b5d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464749"
---
# <a name="list-resources"></a><span data-ttu-id="930cd-107">Список ресурсов</span><span class="sxs-lookup"><span data-stu-id="930cd-107">List resources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="930cd-108">ПереЧислите ресурсы, связанные с этой отправкой.</span><span class="sxs-lookup"><span data-stu-id="930cd-108">List the resources associated with this submission.</span></span> <span data-ttu-id="930cd-109">Объект **субмиссионресаурце** является оболочкой для фактического объекта ресурса, над которым работает учащийся.</span><span class="sxs-lookup"><span data-stu-id="930cd-109">The **submissionResource** object is a wrapper around the actual resource object the student is working on.</span></span> <span data-ttu-id="930cd-110">Кроме того, обертка содержит указатель на ресурсы назначения, который был скопирован из назначения во время процесса Assign.</span><span class="sxs-lookup"><span data-stu-id="930cd-110">The wrapper also includes a pointer to the resources on the assignment if this was copied from the assignment during the assign process.</span></span> <span data-ttu-id="930cd-111">Эти ресурсы являются рабочей копией назначения.</span><span class="sxs-lookup"><span data-stu-id="930cd-111">These resources are the working copy of the assignment.</span></span> <span data-ttu-id="930cd-112">**Субмиттедресаурцес** — это ресурсы, которые официально передаются на производительность.</span><span class="sxs-lookup"><span data-stu-id="930cd-112">The **submittedResources** are the resources that have officially been submitted to be graded.</span></span>

## <a name="permissions"></a><span data-ttu-id="930cd-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="930cd-113">Permissions</span></span>
<span data-ttu-id="930cd-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="930cd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="930cd-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="930cd-116">Permission type</span></span>      | <span data-ttu-id="930cd-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="930cd-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="930cd-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="930cd-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="930cd-119">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="930cd-119">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="930cd-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="930cd-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="930cd-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="930cd-121">Not supported.</span></span>   |
|<span data-ttu-id="930cd-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="930cd-122">Application</span></span> | <span data-ttu-id="930cd-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="930cd-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="930cd-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="930cd-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /educationClasses/assignments/{id}/submissions/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="930cd-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="930cd-125">Optional query parameters</span></span>
<span data-ttu-id="930cd-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="930cd-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="930cd-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="930cd-127">Request headers</span></span>
| <span data-ttu-id="930cd-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="930cd-128">Header</span></span>       | <span data-ttu-id="930cd-129">Значение</span><span class="sxs-lookup"><span data-stu-id="930cd-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="930cd-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="930cd-130">Authorization</span></span>  | <span data-ttu-id="930cd-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="930cd-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="930cd-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="930cd-133">Request body</span></span>
<span data-ttu-id="930cd-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="930cd-134">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="930cd-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="930cd-135">Response</span></span>
<span data-ttu-id="930cd-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [едукатионсубмиссионресаурце](../resources/educationsubmissionresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="930cd-136">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="930cd-137">Пример</span><span class="sxs-lookup"><span data-stu-id="930cd-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="930cd-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="930cd-138">Request</span></span>
<span data-ttu-id="930cd-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="930cd-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments/<id>/submissions/<id>/resources
```
##### <a name="response"></a><span data-ttu-id="930cd-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="930cd-140">Response</span></span>
<span data-ttu-id="930cd-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="930cd-141">The following is an example of the response.</span></span> 

><span data-ttu-id="930cd-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="930cd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-list-resources.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
