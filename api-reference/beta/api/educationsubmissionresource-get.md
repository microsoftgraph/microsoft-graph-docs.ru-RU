---
title: Получение Едукатионсубмиссионресаурце
description: Получает свойства определенного ресурса, связанного с отправкой. Этот ресурс находится в списке ресурсов "Рабочий" и должен рассматриваться в процессе работы студентом. Этот ресурс упаковывается с возможной обратной указателем на ресурс назначения, если он был скопирован из назначения.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b76d697afa842fe5315792d803e9b704a628a0b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464686"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="fa067-105">Получение Едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="fa067-105">Get educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa067-106">Получает свойства определенного ресурса, связанного с отправкой.</span><span class="sxs-lookup"><span data-stu-id="fa067-106">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="fa067-107">Этот ресурс находится в списке ресурсов "Рабочий" и должен рассматриваться в процессе работы студентом.</span><span class="sxs-lookup"><span data-stu-id="fa067-107">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="fa067-108">Этот ресурс упаковывается с возможной обратной указателем на ресурс назначения, если он был скопирован из назначения.</span><span class="sxs-lookup"><span data-stu-id="fa067-108">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa067-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa067-109">Permissions</span></span>
<span data-ttu-id="fa067-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa067-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa067-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa067-112">Permission type</span></span>      | <span data-ttu-id="fa067-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa067-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa067-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa067-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="fa067-115">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa067-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="fa067-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa067-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fa067-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa067-117">Not supported.</span></span>  |
|<span data-ttu-id="fa067-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa067-118">Application</span></span> | <span data-ttu-id="fa067-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa067-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fa067-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa067-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fa067-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fa067-121">Optional query parameters</span></span>
<span data-ttu-id="fa067-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fa067-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa067-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa067-123">Request headers</span></span>
| <span data-ttu-id="fa067-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa067-124">Header</span></span>       | <span data-ttu-id="fa067-125">Значение</span><span class="sxs-lookup"><span data-stu-id="fa067-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fa067-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa067-126">Authorization</span></span>  | <span data-ttu-id="fa067-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa067-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fa067-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa067-129">Request body</span></span>
<span data-ttu-id="fa067-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa067-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fa067-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa067-131">Response</span></span>
<span data-ttu-id="fa067-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [едукатионсубмиссионресаурце](../resources/educationsubmissionresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa067-132">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fa067-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fa067-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa067-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa067-134">Request</span></span>
<span data-ttu-id="fa067-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa067-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmissionresource"
}-->
```http 
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="fa067-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa067-136">Response</span></span>
<span data-ttu-id="fa067-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa067-137">The following is an example of the response.</span></span> 

><span data-ttu-id="fa067-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa067-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmissionresource-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
