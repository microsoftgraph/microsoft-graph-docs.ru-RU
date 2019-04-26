---
title: Обновление Едукатионассигнментресаурце
description: 'Обновление свойств ресурса, связанного с назначением. Изменять объекты ресурсов назначения могут только преподаватели в классе.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d3ce0db2353d91f17f059fe8a2dfd9d6c775e1e2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324699"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="2e87b-104">Обновление Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="2e87b-104">Update educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e87b-105">Обновление свойств ресурса, связанного с назначением.</span><span class="sxs-lookup"><span data-stu-id="2e87b-105">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="2e87b-106">Изменять объекты ресурсов назначения могут только преподаватели в классе.</span><span class="sxs-lookup"><span data-stu-id="2e87b-106">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="2e87b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2e87b-107">Permissions</span></span>
<span data-ttu-id="2e87b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e87b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e87b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2e87b-110">Permission type</span></span>      | <span data-ttu-id="2e87b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2e87b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e87b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2e87b-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="2e87b-113">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e87b-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="2e87b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2e87b-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2e87b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e87b-115">Not supported.</span></span>  |
|<span data-ttu-id="2e87b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2e87b-116">Application</span></span> | <span data-ttu-id="2e87b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e87b-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2e87b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2e87b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2e87b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2e87b-119">Request headers</span></span>
| <span data-ttu-id="2e87b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2e87b-120">Header</span></span>       | <span data-ttu-id="2e87b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2e87b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2e87b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2e87b-122">Authorization</span></span>  | <span data-ttu-id="2e87b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2e87b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2e87b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2e87b-125">Content-Type</span></span>  | <span data-ttu-id="2e87b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e87b-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2e87b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2e87b-127">Request body</span></span>
<span data-ttu-id="2e87b-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="2e87b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2e87b-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="2e87b-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2e87b-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2e87b-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2e87b-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e87b-131">Property</span></span>     | <span data-ttu-id="2e87b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="2e87b-132">Type</span></span>   |<span data-ttu-id="2e87b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="2e87b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e87b-134">Дистрибутефорстудентворк</span><span class="sxs-lookup"><span data-stu-id="2e87b-134">distributeForStudentWork</span></span>|<span data-ttu-id="2e87b-135">Логический</span><span class="sxs-lookup"><span data-stu-id="2e87b-135">Boolean</span></span>| <span data-ttu-id="2e87b-136">Указывает, следует ли копировать этот ресурс в объект ресурса каждого учащегося при публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="2e87b-136">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="2e87b-137">resource</span><span class="sxs-lookup"><span data-stu-id="2e87b-137">resource</span></span>|<span data-ttu-id="2e87b-138">Едукатионресаурце</span><span class="sxs-lookup"><span data-stu-id="2e87b-138">educationResource</span></span>| <span data-ttu-id="2e87b-139">Объект Resource.</span><span class="sxs-lookup"><span data-stu-id="2e87b-139">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="2e87b-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e87b-140">Response</span></span>
<span data-ttu-id="2e87b-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [едукатионассигнментресаурце](../resources/educationassignmentresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2e87b-141">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2e87b-142">Пример</span><span class="sxs-lookup"><span data-stu-id="2e87b-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e87b-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="2e87b-143">Request</span></span>
<span data-ttu-id="2e87b-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2e87b-144">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2e87b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="2e87b-145">Response</span></span>
<span data-ttu-id="2e87b-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2e87b-146">The following is an example of the response.</span></span> 

><span data-ttu-id="2e87b-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2e87b-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2e87b-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2e87b-148">All of the properties will be returned from an actual call.</span></span>


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
  "suppressions": []
}
-->
