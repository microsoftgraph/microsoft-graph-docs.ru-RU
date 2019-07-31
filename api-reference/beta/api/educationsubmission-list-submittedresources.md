---
title: Список Субмиттедресаурцес
description: Перечислите ресурсы, которые были отправлены официально. Студент, владеющий отправкой, не может изменить отправленный список без повторной отправки назначения. Это оболочка для реального ресурса и может содержать указатель на фактический ресурс назначения, если этот ресурс был скопирован из назначения.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 371302640df794465764755492088ec2015278ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955127"
---
# <a name="list-submittedresources"></a><span data-ttu-id="9f782-105">Список Субмиттедресаурцес</span><span class="sxs-lookup"><span data-stu-id="9f782-105">List submittedResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f782-106">Перечислите ресурсы, которые были отправлены официально.</span><span class="sxs-lookup"><span data-stu-id="9f782-106">List the resources that have officially been submitted for grading.</span></span> <span data-ttu-id="9f782-107">Студент, владеющий отправкой, не может изменить отправленный список без повторной отправки назначения.</span><span class="sxs-lookup"><span data-stu-id="9f782-107">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="9f782-108">Это оболочка для реального ресурса и может содержать указатель на фактический ресурс назначения, если этот ресурс был скопирован из назначения.</span><span class="sxs-lookup"><span data-stu-id="9f782-108">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f782-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f782-109">Permissions</span></span>
<span data-ttu-id="9f782-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f782-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f782-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f782-112">Permission type</span></span>      | <span data-ttu-id="9f782-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f782-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f782-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f782-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="9f782-115">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f782-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="9f782-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f782-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9f782-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f782-117">Not supported.</span></span>  |
|<span data-ttu-id="9f782-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f782-118">Application</span></span> | <span data-ttu-id="9f782-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f782-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9f782-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f782-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9f782-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9f782-121">Optional query parameters</span></span>
<span data-ttu-id="9f782-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9f782-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f782-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f782-123">Request headers</span></span>
| <span data-ttu-id="9f782-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f782-124">Header</span></span>       | <span data-ttu-id="9f782-125">Значение</span><span class="sxs-lookup"><span data-stu-id="9f782-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9f782-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f782-126">Authorization</span></span>  | <span data-ttu-id="9f782-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f782-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f782-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f782-129">Request body</span></span>
<span data-ttu-id="9f782-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f782-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9f782-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f782-131">Response</span></span>
<span data-ttu-id="9f782-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [едукатионсубмиссионресаурце](../resources/educationsubmissionresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f782-132">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9f782-133">Пример</span><span class="sxs-lookup"><span data-stu-id="9f782-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f782-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f782-134">Request</span></span>
<span data-ttu-id="9f782-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f782-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources
```
##### <a name="response"></a><span data-ttu-id="9f782-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f782-136">Response</span></span>
<span data-ttu-id="9f782-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9f782-137">The following is an example of the response.</span></span> 

><span data-ttu-id="9f782-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f782-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource",
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
        "link": "https://www.microsoft.com
        },
        "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource" 
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List submittedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
