---
title: Создание educationSubmissionResource
description: 'Добавляет ресурс в список ресурсов. Это действие можно выполнить только с учебы, которому назначена эта отправки. Это действие не будет выполнено, если флаг **allowStudentsToAddResources** не установлен в значение true. Если вызывающий объект должен создать новый файловый ресурс, необходимо отправить этот файл в папку ресурсов, который связан с подачи. Если файл не существует или не находится в папке, запрос POST завершится с ошибкой. '
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 585ece0dd8239c5a3107420b88cf2103fe5fb7eb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888118"
---
# <a name="create-educationsubmissionresource"></a><span data-ttu-id="85aa0-107">Создание educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="85aa0-107">Create educationSubmissionResource</span></span>

> <span data-ttu-id="85aa0-108">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="85aa0-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85aa0-109">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85aa0-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85aa0-110">Добавляет ресурс в список ресурсов.</span><span class="sxs-lookup"><span data-stu-id="85aa0-110">Adds a resource to the resources list.</span></span> <span data-ttu-id="85aa0-111">Это действие можно выполнить только с учебы, которому назначена эта отправки.</span><span class="sxs-lookup"><span data-stu-id="85aa0-111">This action can only be done by the student to whom this submission is assigned.</span></span> <span data-ttu-id="85aa0-112">Это действие не будет выполнено, если флаг **allowStudentsToAddResources** не установлен в значение true.</span><span class="sxs-lookup"><span data-stu-id="85aa0-112">This action will not succeed if the **allowStudentsToAddResources** flag is not set to true.</span></span> <span data-ttu-id="85aa0-113">Если вызывающий объект должен создать новый файловый ресурс, необходимо отправить этот файл в папку ресурсов, который связан с подачи.</span><span class="sxs-lookup"><span data-stu-id="85aa0-113">If the caller wants to create a new file-based resource, the file must be uploaded to the resources folder that is associated with the submission.</span></span> <span data-ttu-id="85aa0-114">Если файл не существует или не находится в папке, запрос POST завершится с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="85aa0-114">If the file does not exist or is not in that folder, the POST request will fail.</span></span> 

## <a name="permissions"></a><span data-ttu-id="85aa0-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85aa0-115">Permissions</span></span>
<span data-ttu-id="85aa0-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85aa0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85aa0-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85aa0-118">Permission type</span></span>      | <span data-ttu-id="85aa0-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85aa0-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85aa0-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85aa0-120">Delegated (work or school account)</span></span> |  <span data-ttu-id="85aa0-121">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85aa0-121">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="85aa0-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85aa0-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85aa0-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85aa0-123">Not supported.</span></span>  |
|<span data-ttu-id="85aa0-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85aa0-124">Application</span></span> | <span data-ttu-id="85aa0-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85aa0-125">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="85aa0-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85aa0-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/resources

```
## <a name="request-headers"></a><span data-ttu-id="85aa0-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85aa0-127">Request headers</span></span>
| <span data-ttu-id="85aa0-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85aa0-128">Header</span></span>       | <span data-ttu-id="85aa0-129">Значение</span><span class="sxs-lookup"><span data-stu-id="85aa0-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="85aa0-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85aa0-130">Authorization</span></span>  | <span data-ttu-id="85aa0-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85aa0-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="85aa0-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85aa0-133">Content-Type</span></span>  | <span data-ttu-id="85aa0-134">application/json</span><span class="sxs-lookup"><span data-stu-id="85aa0-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="85aa0-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85aa0-135">Request body</span></span>
<span data-ttu-id="85aa0-136">В тексте запроса укажите представление объекта [educationSubmissionResource](../resources/educationsubmissionresource.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="85aa0-136">In the request body, supply a JSON representation of the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="85aa0-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="85aa0-137">Response</span></span>
<span data-ttu-id="85aa0-138">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [educationSubmissionResource](../resources/educationsubmissionresource.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="85aa0-138">If successful, this method returns a `201 Created` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85aa0-139">Пример</span><span class="sxs-lookup"><span data-stu-id="85aa0-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85aa0-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="85aa0-140">Request</span></span>
<span data-ttu-id="85aa0-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85aa0-141">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="85aa0-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="85aa0-142">Response</span></span>
<span data-ttu-id="85aa0-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="85aa0-143">The following is an example of the response.</span></span> 

><span data-ttu-id="85aa0-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85aa0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
