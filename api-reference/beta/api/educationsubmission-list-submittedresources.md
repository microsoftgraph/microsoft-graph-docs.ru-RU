---
title: Список, представленныйРесурсеи
description: Список ресурсов, официально отправленных для классификации. Учащийся, которому принадлежит отправка, не может изменить представленный список без повторного отправки задания. Это оболочка вокруг реального ресурса и может содержать указатель обратно на фактический ресурс назначения, если этот ресурс был скопирован из назначения.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 861ee3371517d95e89c9077d6e139202d370a917
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061842"
---
# <a name="list-submittedresources"></a><span data-ttu-id="4a5bc-105">Список, представленныйРесурсеи</span><span class="sxs-lookup"><span data-stu-id="4a5bc-105">List submittedResources</span></span>

<span data-ttu-id="4a5bc-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a5bc-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a5bc-107">Список ресурсов, официально отправленных для классификации.</span><span class="sxs-lookup"><span data-stu-id="4a5bc-107">List the resources that have officially been submitted for grading.</span></span> <span data-ttu-id="4a5bc-108">Учащийся, которому принадлежит отправка, не может изменить представленный список без повторного отправки задания.</span><span class="sxs-lookup"><span data-stu-id="4a5bc-108">The student who owns the submission cannot change the submitted list without resubmitting the assignment.</span></span> <span data-ttu-id="4a5bc-109">Это оболочка вокруг реального ресурса и может содержать указатель обратно на фактический ресурс назначения, если этот ресурс был скопирован из назначения.</span><span class="sxs-lookup"><span data-stu-id="4a5bc-109">This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a5bc-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a5bc-110">Permissions</span></span>
<span data-ttu-id="4a5bc-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a5bc-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a5bc-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a5bc-113">Permission type</span></span>      | <span data-ttu-id="4a5bc-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a5bc-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a5bc-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a5bc-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="4a5bc-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a5bc-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="4a5bc-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a5bc-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4a5bc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a5bc-118">Not supported.</span></span>  |
|<span data-ttu-id="4a5bc-119">Приложение\*</span><span class="sxs-lookup"><span data-stu-id="4a5bc-119">Application\*</span></span> | <span data-ttu-id="4a5bc-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a5bc-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="4a5bc-121">\*Разрешения приложения в настоящее время доступны только для частных пользователей предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="4a5bc-121">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="4a5bc-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a5bc-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4a5bc-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4a5bc-123">Optional query parameters</span></span>
<span data-ttu-id="4a5bc-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4a5bc-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a5bc-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a5bc-125">Request headers</span></span>
| <span data-ttu-id="4a5bc-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a5bc-126">Header</span></span>       | <span data-ttu-id="4a5bc-127">Значение</span><span class="sxs-lookup"><span data-stu-id="4a5bc-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4a5bc-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a5bc-128">Authorization</span></span>  | <span data-ttu-id="4a5bc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a5bc-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4a5bc-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a5bc-131">Request body</span></span>
<span data-ttu-id="4a5bc-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a5bc-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4a5bc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a5bc-133">Response</span></span>
<span data-ttu-id="4a5bc-134">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [educationSubmissionResource](../resources/educationsubmissionresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4a5bc-134">If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a5bc-135">Пример</span><span class="sxs-lookup"><span data-stu-id="4a5bc-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a5bc-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a5bc-136">Request</span></span>
<span data-ttu-id="4a5bc-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a5bc-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources
```
##### <a name="response"></a><span data-ttu-id="4a5bc-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a5bc-138">Response</span></span>
<span data-ttu-id="4a5bc-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4a5bc-139">The following is an example of the response.</span></span> 

><span data-ttu-id="4a5bc-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4a5bc-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
          "link": "https://www.microsoft.com"
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
