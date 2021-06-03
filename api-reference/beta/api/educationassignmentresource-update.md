---
title: Обновление educationAssignmentResource
description: 'Обновление свойств ресурса, связанного с назначением. Только преподаватели в классе могут изменять объекты ресурсов назначения.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5dae821a6dc22aa108bceee44c4958e3deb7f129
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52733006"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="8b30a-104">Обновление educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="8b30a-104">Update educationAssignmentResource</span></span>

<span data-ttu-id="8b30a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b30a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b30a-106">Обновление свойств ресурса, связанного с назначением.</span><span class="sxs-lookup"><span data-stu-id="8b30a-106">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="8b30a-107">Только преподаватели в классе могут изменять объекты ресурсов назначения.</span><span class="sxs-lookup"><span data-stu-id="8b30a-107">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="8b30a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b30a-108">Permissions</span></span>
<span data-ttu-id="8b30a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b30a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b30a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b30a-111">Permission type</span></span>      | <span data-ttu-id="8b30a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b30a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b30a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b30a-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="8b30a-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b30a-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="8b30a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b30a-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8b30a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b30a-116">Not supported.</span></span>  |
|<span data-ttu-id="8b30a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b30a-117">Application</span></span> | <span data-ttu-id="8b30a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b30a-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8b30a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b30a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8b30a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b30a-120">Request headers</span></span>
| <span data-ttu-id="8b30a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b30a-121">Header</span></span>       | <span data-ttu-id="8b30a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8b30a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8b30a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b30a-123">Authorization</span></span>  | <span data-ttu-id="8b30a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b30a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8b30a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b30a-126">Content-Type</span></span>  | <span data-ttu-id="8b30a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8b30a-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8b30a-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b30a-128">Request body</span></span>
<span data-ttu-id="8b30a-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="8b30a-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8b30a-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="8b30a-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8b30a-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8b30a-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8b30a-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b30a-132">Property</span></span>     | <span data-ttu-id="8b30a-133">Тип</span><span class="sxs-lookup"><span data-stu-id="8b30a-133">Type</span></span>   |<span data-ttu-id="8b30a-134">Описание</span><span class="sxs-lookup"><span data-stu-id="8b30a-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b30a-135">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="8b30a-135">distributeForStudentWork</span></span>|<span data-ttu-id="8b30a-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b30a-136">Boolean</span></span>| <span data-ttu-id="8b30a-137">Указывает, следует ли скопировать этот ресурс на объект ресурсов каждого учащегося при публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="8b30a-137">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="8b30a-138">resource</span><span class="sxs-lookup"><span data-stu-id="8b30a-138">resource</span></span>|<span data-ttu-id="8b30a-139">educationResource</span><span class="sxs-lookup"><span data-stu-id="8b30a-139">educationResource</span></span>| <span data-ttu-id="8b30a-140">Объект Resource.</span><span class="sxs-lookup"><span data-stu-id="8b30a-140">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="8b30a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b30a-141">Response</span></span>
<span data-ttu-id="8b30a-142">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [educationAssignmentResource](../resources/educationassignmentresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8b30a-142">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b30a-143">Пример</span><span class="sxs-lookup"><span data-stu-id="8b30a-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b30a-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b30a-144">Request</span></span>
<span data-ttu-id="8b30a-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b30a-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b30a-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b30a-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
# <a name="c"></a>[<span data-ttu-id="8b30a-147">C#</span><span class="sxs-lookup"><span data-stu-id="8b30a-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b30a-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b30a-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b30a-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b30a-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b30a-150">Java</span><span class="sxs-lookup"><span data-stu-id="8b30a-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8b30a-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b30a-151">Response</span></span>
<span data-ttu-id="8b30a-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8b30a-152">The following is an example of the response.</span></span> 

><span data-ttu-id="8b30a-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8b30a-153">**Note:** The response object shown here might be shortened for readability.</span></span>


<!-- {
  "blockType": "response",
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


