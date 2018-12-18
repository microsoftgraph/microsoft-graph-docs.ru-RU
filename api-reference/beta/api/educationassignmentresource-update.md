---
title: Обновление educationAssignmentResource
description: 'Обновление свойств ресурса, связанного с назначением. Учителя только в классе можно изменить объекты назначения ресурсов.  '
author: dipakboyed
ms.openlocfilehash: 68c8f471462c489e9e655a1642731be3a8700ba4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343220"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="32955-104">Обновление educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="32955-104">Update educationAssignmentResource</span></span>

> <span data-ttu-id="32955-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="32955-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32955-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32955-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32955-107">Обновление свойств ресурса, связанного с назначением.</span><span class="sxs-lookup"><span data-stu-id="32955-107">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="32955-108">Учителя только в классе можно изменить объекты назначения ресурсов.</span><span class="sxs-lookup"><span data-stu-id="32955-108">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="32955-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32955-109">Permissions</span></span>
<span data-ttu-id="32955-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32955-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32955-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32955-112">Permission type</span></span>      | <span data-ttu-id="32955-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32955-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32955-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32955-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="32955-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32955-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="32955-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32955-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="32955-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32955-117">Not supported.</span></span>  |
|<span data-ttu-id="32955-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32955-118">Application</span></span> | <span data-ttu-id="32955-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32955-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="32955-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32955-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="32955-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32955-121">Request headers</span></span>
| <span data-ttu-id="32955-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="32955-122">Header</span></span>       | <span data-ttu-id="32955-123">Значение</span><span class="sxs-lookup"><span data-stu-id="32955-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="32955-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32955-124">Authorization</span></span>  | <span data-ttu-id="32955-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32955-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="32955-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32955-127">Content-Type</span></span>  | <span data-ttu-id="32955-128">application/json</span><span class="sxs-lookup"><span data-stu-id="32955-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="32955-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32955-129">Request body</span></span>
<span data-ttu-id="32955-130">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="32955-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="32955-131">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="32955-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="32955-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="32955-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="32955-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="32955-133">Property</span></span>     | <span data-ttu-id="32955-134">Тип</span><span class="sxs-lookup"><span data-stu-id="32955-134">Type</span></span>   |<span data-ttu-id="32955-135">Описание</span><span class="sxs-lookup"><span data-stu-id="32955-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32955-136">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="32955-136">distributeForStudentWork</span></span>|<span data-ttu-id="32955-137">Boolean.</span><span class="sxs-lookup"><span data-stu-id="32955-137">Boolean</span></span>| <span data-ttu-id="32955-138">Указывает, следует ли скопировать этот ресурс объект ресурсов каждого студента при публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="32955-138">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="32955-139">resource</span><span class="sxs-lookup"><span data-stu-id="32955-139">resource</span></span>|<span data-ttu-id="32955-140">educationResource</span><span class="sxs-lookup"><span data-stu-id="32955-140">educationResource</span></span>| <span data-ttu-id="32955-141">Объект ресурса.</span><span class="sxs-lookup"><span data-stu-id="32955-141">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="32955-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="32955-142">Response</span></span>
<span data-ttu-id="32955-143">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [educationAssignmentResource](../resources/educationassignmentresource.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="32955-143">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="32955-144">Пример</span><span class="sxs-lookup"><span data-stu-id="32955-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32955-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="32955-145">Request</span></span>
<span data-ttu-id="32955-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="32955-146">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="32955-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="32955-147">Response</span></span>
<span data-ttu-id="32955-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="32955-148">The following is an example of the response.</span></span> 

><span data-ttu-id="32955-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="32955-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="32955-150">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="32955-150">All of the properties will be returned from an actual call.</span></span>


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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationassignmentresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
