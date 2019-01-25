---
title: Создание educationSubmissionResource
description: 'Добавляет ресурс в список ресурсов. Это действие можно выполнить только с учебы, которому назначена эта отправки. Это действие не будет выполнено, если флаг **allowStudentsToAddResources** не установлен в значение true. Если вызывающий объект должен создать новый файловый ресурс, необходимо отправить этот файл в папку ресурсов, который связан с подачи. Если файл не существует или не находится в папке, запрос POST завершится с ошибкой. '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: da0860d5b5f19a84643a05a88aaeb74651e2d8ea
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511732"
---
# <a name="create-educationsubmissionresource"></a><span data-ttu-id="73cfe-107">Создание educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="73cfe-107">Create educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73cfe-108">Добавляет ресурс в список ресурсов.</span><span class="sxs-lookup"><span data-stu-id="73cfe-108">Adds a resource to the resources list.</span></span> <span data-ttu-id="73cfe-109">Это действие можно выполнить только с учебы, которому назначена эта отправки.</span><span class="sxs-lookup"><span data-stu-id="73cfe-109">This action can only be done by the student to whom this submission is assigned.</span></span> <span data-ttu-id="73cfe-110">Это действие не будет выполнено, если флаг **allowStudentsToAddResources** не установлен в значение true.</span><span class="sxs-lookup"><span data-stu-id="73cfe-110">This action will not succeed if the **allowStudentsToAddResources** flag is not set to true.</span></span> <span data-ttu-id="73cfe-111">Если вызывающий объект должен создать новый файловый ресурс, необходимо отправить этот файл в папку ресурсов, который связан с подачи.</span><span class="sxs-lookup"><span data-stu-id="73cfe-111">If the caller wants to create a new file-based resource, the file must be uploaded to the resources folder that is associated with the submission.</span></span> <span data-ttu-id="73cfe-112">Если файл не существует или не находится в папке, запрос POST завершится с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="73cfe-112">If the file does not exist or is not in that folder, the POST request will fail.</span></span> 

## <a name="permissions"></a><span data-ttu-id="73cfe-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="73cfe-113">Permissions</span></span>
<span data-ttu-id="73cfe-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73cfe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73cfe-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="73cfe-116">Permission type</span></span>      | <span data-ttu-id="73cfe-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="73cfe-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73cfe-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="73cfe-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="73cfe-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73cfe-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="73cfe-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="73cfe-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73cfe-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73cfe-121">Not supported.</span></span>  |
|<span data-ttu-id="73cfe-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="73cfe-122">Application</span></span> | <span data-ttu-id="73cfe-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73cfe-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="73cfe-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="73cfe-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/resources

```
## <a name="request-headers"></a><span data-ttu-id="73cfe-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="73cfe-125">Request headers</span></span>
| <span data-ttu-id="73cfe-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="73cfe-126">Header</span></span>       | <span data-ttu-id="73cfe-127">Значение</span><span class="sxs-lookup"><span data-stu-id="73cfe-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="73cfe-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="73cfe-128">Authorization</span></span>  | <span data-ttu-id="73cfe-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="73cfe-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="73cfe-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73cfe-131">Content-Type</span></span>  | <span data-ttu-id="73cfe-132">application/json</span><span class="sxs-lookup"><span data-stu-id="73cfe-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="73cfe-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="73cfe-133">Request body</span></span>
<span data-ttu-id="73cfe-134">В тексте запроса укажите представление объекта [educationSubmissionResource](../resources/educationsubmissionresource.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="73cfe-134">In the request body, supply a JSON representation of the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="73cfe-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="73cfe-135">Response</span></span>
<span data-ttu-id="73cfe-136">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [educationSubmissionResource](../resources/educationsubmissionresource.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="73cfe-136">If successful, this method returns a `201 Created` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73cfe-137">Пример</span><span class="sxs-lookup"><span data-stu-id="73cfe-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73cfe-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="73cfe-138">Request</span></span>
<span data-ttu-id="73cfe-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="73cfe-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationsubmissionresource_from_educationsubmission"
}-->
```
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources
Content-type: application/json
Content-length: 1097

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
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
  "@odata.type": "microsoft.graph.educationResource"
}

```

##### <a name="response"></a><span data-ttu-id="73cfe-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="73cfe-140">Response</span></span>
<span data-ttu-id="73cfe-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="73cfe-141">The following is an example of the response.</span></span> 

><span data-ttu-id="73cfe-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="73cfe-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
} -->
```http
HTTP/1.1 201 Created
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
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6",
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-post-resources.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
