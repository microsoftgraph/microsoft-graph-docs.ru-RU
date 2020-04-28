---
title: Обновление Едукатионассигнментресаурце
description: 'Обновление свойств ресурса, связанного с назначением. Изменять объекты ресурсов назначения могут только преподаватели в классе.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: cb210affa5d98bdbc9a5cd012adc20a5c4ac49ea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427090"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="e8b4b-104">Обновление Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="e8b4b-104">Update educationAssignmentResource</span></span>

<span data-ttu-id="e8b4b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8b4b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8b4b-106">Обновление свойств ресурса, связанного с назначением.</span><span class="sxs-lookup"><span data-stu-id="e8b4b-106">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="e8b4b-107">Изменять объекты ресурсов назначения могут только преподаватели в классе.</span><span class="sxs-lookup"><span data-stu-id="e8b4b-107">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="e8b4b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8b4b-108">Permissions</span></span>
<span data-ttu-id="e8b4b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8b4b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8b4b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8b4b-111">Permission type</span></span>      | <span data-ttu-id="e8b4b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8b4b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8b4b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8b4b-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="e8b4b-114">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8b4b-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="e8b4b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8b4b-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e8b4b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8b4b-116">Not supported.</span></span>  |
|<span data-ttu-id="e8b4b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8b4b-117">Application</span></span> | <span data-ttu-id="e8b4b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8b4b-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e8b4b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8b4b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e8b4b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8b4b-120">Request headers</span></span>
| <span data-ttu-id="e8b4b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8b4b-121">Header</span></span>       | <span data-ttu-id="e8b4b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e8b4b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e8b4b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8b4b-123">Authorization</span></span>  | <span data-ttu-id="e8b4b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8b4b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e8b4b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e8b4b-126">Content-Type</span></span>  | <span data-ttu-id="e8b4b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e8b4b-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e8b4b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8b4b-128">Request body</span></span>
<span data-ttu-id="e8b4b-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="e8b4b-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e8b4b-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="e8b4b-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e8b4b-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e8b4b-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e8b4b-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8b4b-132">Property</span></span>     | <span data-ttu-id="e8b4b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="e8b4b-133">Type</span></span>   |<span data-ttu-id="e8b4b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="e8b4b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8b4b-135">дистрибутефорстудентворк</span><span class="sxs-lookup"><span data-stu-id="e8b4b-135">distributeForStudentWork</span></span>|<span data-ttu-id="e8b4b-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8b4b-136">Boolean</span></span>| <span data-ttu-id="e8b4b-137">Указывает, следует ли копировать этот ресурс в объект ресурса каждого учащегося при публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="e8b4b-137">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="e8b4b-138">resource</span><span class="sxs-lookup"><span data-stu-id="e8b4b-138">resource</span></span>|<span data-ttu-id="e8b4b-139">едукатионресаурце</span><span class="sxs-lookup"><span data-stu-id="e8b4b-139">educationResource</span></span>| <span data-ttu-id="e8b4b-140">Объект Resource.</span><span class="sxs-lookup"><span data-stu-id="e8b4b-140">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="e8b4b-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="e8b4b-141">Response</span></span>
<span data-ttu-id="e8b4b-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [едукатионассигнментресаурце](../resources/educationassignmentresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8b4b-142">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8b4b-143">Пример</span><span class="sxs-lookup"><span data-stu-id="e8b4b-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8b4b-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8b4b-144">Request</span></span>
<span data-ttu-id="e8b4b-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8b4b-145">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="e8b4b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8b4b-146">Response</span></span>
<span data-ttu-id="e8b4b-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e8b4b-147">The following is an example of the response.</span></span> 

><span data-ttu-id="e8b4b-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e8b4b-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e8b4b-149">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8b4b-149">All of the properties will be returned from an actual call.</span></span>


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
