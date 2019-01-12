---
title: Получение educationAssignmentResource
description: 'Получение свойств определенного ресурса по назначению.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ef673726bab6124ea1337d9175a3f0fbfd3879eb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940654"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="9f566-103">Получение educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="9f566-103">Get educationAssignmentResource</span></span>

> <span data-ttu-id="9f566-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9f566-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f566-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f566-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f566-106">Получение свойств определенного ресурса по назначению.</span><span class="sxs-lookup"><span data-stu-id="9f566-106">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="9f566-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f566-107">Permissions</span></span>
<span data-ttu-id="9f566-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f566-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f566-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f566-110">Permission type</span></span>      | <span data-ttu-id="9f566-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f566-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f566-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f566-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9f566-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9f566-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="9f566-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f566-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9f566-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f566-115">Not supported.</span></span>  |
|<span data-ttu-id="9f566-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f566-116">Application</span></span> |  <span data-ttu-id="9f566-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f566-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9f566-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f566-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9f566-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9f566-119">Optional query parameters</span></span>
<span data-ttu-id="9f566-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9f566-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f566-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f566-121">Request headers</span></span>
| <span data-ttu-id="9f566-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f566-122">Header</span></span>       | <span data-ttu-id="9f566-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9f566-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9f566-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f566-124">Authorization</span></span>  | <span data-ttu-id="9f566-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f566-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f566-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f566-127">Request body</span></span>
<span data-ttu-id="9f566-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f566-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9f566-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f566-129">Response</span></span>
<span data-ttu-id="9f566-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [educationAssignmentResource](../resources/educationassignmentresource.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9f566-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9f566-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9f566-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f566-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f566-132">Request</span></span>
<span data-ttu-id="9f566-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f566-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="9f566-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f566-134">Response</span></span>
<span data-ttu-id="9f566-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9f566-135">The following is an example of the response.</span></span> 

><span data-ttu-id="9f566-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9f566-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9f566-137">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f566-137">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 842

{
  "distributeForStudentWork": true,
  "id": "22002",
  "resource": {
    "createdBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "createdDateTime": "2014-01-01T00:00:00Z",
    "displayName": "Excel workbook 1",
    "lastModifiedBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "lastModifiedDateTime": "2014-01-01T00:00:00Z"
  }
}
    
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
