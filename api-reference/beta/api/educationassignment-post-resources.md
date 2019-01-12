---
title: Создание educationAssignmentResource
description: создается OData.Type, чтобы указать, какой тип ресурсов. Обратите внимание, что файловым ресурсам, сначала нужно передать для назначения **resourceFolder**.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 46233ec2f8c8acb698dd707f7df06edaca70fec4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965392"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="ad639-104">Создание educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="ad639-104">Create educationAssignmentResource</span></span>

> <span data-ttu-id="ad639-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ad639-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad639-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad639-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad639-107">Создание [назначения ресурсов](../resources/educationassignmentresource.md).</span><span class="sxs-lookup"><span data-stu-id="ad639-107">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="ad639-108">Сам ресурс имеет @odata.type которое указывает тип ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ad639-108">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="ad639-109">Обратите внимание, что файловым ресурсам, сначала нужно передать для назначения **resourceFolder**.</span><span class="sxs-lookup"><span data-stu-id="ad639-109">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad639-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad639-110">Permissions</span></span>
<span data-ttu-id="ad639-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad639-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad639-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad639-113">Permission type</span></span>      | <span data-ttu-id="ad639-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad639-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad639-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad639-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="ad639-116">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad639-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="ad639-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad639-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="ad639-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad639-118">Not supported.</span></span>  |
|<span data-ttu-id="ad639-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad639-119">Application</span></span> | <span data-ttu-id="ad639-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad639-120">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="ad639-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad639-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="ad639-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad639-122">Request headers</span></span>
| <span data-ttu-id="ad639-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad639-123">Header</span></span>       | <span data-ttu-id="ad639-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ad639-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ad639-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad639-125">Authorization</span></span>  | <span data-ttu-id="ad639-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad639-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ad639-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad639-128">Content-Type</span></span>  | <span data-ttu-id="ad639-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ad639-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ad639-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ad639-130">Request body</span></span>
<span data-ttu-id="ad639-131">В тексте запроса укажите представление объекта [educationAssignmentResource](../resources/educationassignmentresource.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="ad639-131">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="ad639-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad639-132">Response</span></span>
<span data-ttu-id="ad639-133">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [educationAssignmentResource](../resources/educationassignmentresource.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ad639-133">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad639-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ad639-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad639-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad639-135">Request</span></span>
<span data-ttu-id="ad639-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad639-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationassignmentresource_from_educationassignment"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources
Content-type: application/json
Content-length: 212

{
  "distributeForStudentWork": "false",
  "resource": {
    "displayName": "Bing",
    "link": "https://www.bing.com",
    "@odata.type": "#microsoft.education.assignments.api.educationLinkResource"
  }
}

```
<span data-ttu-id="ad639-137">В тексте запроса укажите представление объекта [educationAssignmentResource](../resources/educationassignmentresource.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="ad639-137">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ad639-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="ad639-138">Response</span></span>
<span data-ttu-id="ad639-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ad639-139">The following is an example of the response.</span></span> 

><span data-ttu-id="ad639-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ad639-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ad639-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad639-141">All of the properties will be returned from an actual call.</span></span>


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 229

{
  "id": "122333",
  "distributeForStudentWork": false,
  "resource": {
    "displayName": "Bing",
    "link": "https://www.bing.com",
    "@odata.type": "#microsoft.education.assignments.api.educationLinkResource"
  }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
