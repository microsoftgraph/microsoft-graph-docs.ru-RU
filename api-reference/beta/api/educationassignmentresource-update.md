---
title: Обновление educationAssignmentResource
description: 'Обновление свойств ресурса, связанного с назначением. Учителя только в классе можно изменить объекты назначения ресурсов.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 34b1c05937f57fe46d5d854d21a7c2e0b68240d2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527957"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="c24c1-104">Обновление educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="c24c1-104">Update educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c24c1-105">Обновление свойств ресурса, связанного с назначением.</span><span class="sxs-lookup"><span data-stu-id="c24c1-105">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="c24c1-106">Учителя только в классе можно изменить объекты назначения ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c24c1-106">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="c24c1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c24c1-107">Permissions</span></span>
<span data-ttu-id="c24c1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c24c1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c24c1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c24c1-110">Permission type</span></span>      | <span data-ttu-id="c24c1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c24c1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c24c1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c24c1-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="c24c1-113">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c24c1-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="c24c1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c24c1-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c24c1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c24c1-115">Not supported.</span></span>  |
|<span data-ttu-id="c24c1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c24c1-116">Application</span></span> | <span data-ttu-id="c24c1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c24c1-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c24c1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c24c1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c24c1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c24c1-119">Request headers</span></span>
| <span data-ttu-id="c24c1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c24c1-120">Header</span></span>       | <span data-ttu-id="c24c1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c24c1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c24c1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c24c1-122">Authorization</span></span>  | <span data-ttu-id="c24c1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c24c1-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c24c1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c24c1-125">Content-Type</span></span>  | <span data-ttu-id="c24c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c24c1-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c24c1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c24c1-127">Request body</span></span>
<span data-ttu-id="c24c1-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="c24c1-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c24c1-129">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="c24c1-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c24c1-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c24c1-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c24c1-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="c24c1-131">Property</span></span>     | <span data-ttu-id="c24c1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c24c1-132">Type</span></span>   |<span data-ttu-id="c24c1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c24c1-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c24c1-134">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="c24c1-134">distributeForStudentWork</span></span>|<span data-ttu-id="c24c1-135">Логическое</span><span class="sxs-lookup"><span data-stu-id="c24c1-135">Boolean</span></span>| <span data-ttu-id="c24c1-136">Указывает, следует ли скопировать этот ресурс объект ресурсов каждого студента при публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="c24c1-136">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="c24c1-137">resource</span><span class="sxs-lookup"><span data-stu-id="c24c1-137">resource</span></span>|<span data-ttu-id="c24c1-138">educationResource</span><span class="sxs-lookup"><span data-stu-id="c24c1-138">educationResource</span></span>| <span data-ttu-id="c24c1-139">Объект Resource</span><span class="sxs-lookup"><span data-stu-id="c24c1-139">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="c24c1-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="c24c1-140">Response</span></span>
<span data-ttu-id="c24c1-141">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [educationAssignmentResource](../resources/educationassignmentresource.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c24c1-141">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c24c1-142">Пример</span><span class="sxs-lookup"><span data-stu-id="c24c1-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c24c1-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="c24c1-143">Request</span></span>
<span data-ttu-id="c24c1-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c24c1-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_educationassignmentresource"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/850f51b7-1df9-4ec0-bd62-64a0214b9cbf
Content-type: application/json
Content-length: 822

{
  "distributeForStudentWork": "false"
}
```
##### <a name="response"></a><span data-ttu-id="c24c1-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="c24c1-145">Response</span></span>
<span data-ttu-id="c24c1-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c24c1-146">The following is an example of the response.</span></span> 

><span data-ttu-id="c24c1-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c24c1-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c24c1-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c24c1-148">All of the properties will be returned from an actual call.</span></span>


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 832

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
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationassignmentresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignmentresource-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
