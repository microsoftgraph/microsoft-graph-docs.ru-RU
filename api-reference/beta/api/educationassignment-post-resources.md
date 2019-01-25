---
title: Создание educationAssignmentResource
description: создается OData.Type, чтобы указать, какой тип ресурсов. Обратите внимание, что файловым ресурсам, сначала нужно передать для назначения **resourceFolder**.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 34e8740336acbef056ec0b3703547de51fdc42ce
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527992"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="236e6-104">Создание educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="236e6-104">Create educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="236e6-105">Создание [назначения ресурсов](../resources/educationassignmentresource.md).</span><span class="sxs-lookup"><span data-stu-id="236e6-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="236e6-106">Сам ресурс имеет @odata.type которое указывает тип ресурсов.</span><span class="sxs-lookup"><span data-stu-id="236e6-106">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="236e6-107">Обратите внимание, что файловым ресурсам, сначала нужно передать для назначения **resourceFolder**.</span><span class="sxs-lookup"><span data-stu-id="236e6-107">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="236e6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="236e6-108">Permissions</span></span>
<span data-ttu-id="236e6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="236e6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="236e6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="236e6-111">Permission type</span></span>      | <span data-ttu-id="236e6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="236e6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="236e6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="236e6-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="236e6-114">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="236e6-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="236e6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="236e6-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="236e6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="236e6-116">Not supported.</span></span>  |
|<span data-ttu-id="236e6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="236e6-117">Application</span></span> | <span data-ttu-id="236e6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="236e6-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="236e6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="236e6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="236e6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="236e6-120">Request headers</span></span>
| <span data-ttu-id="236e6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="236e6-121">Header</span></span>       | <span data-ttu-id="236e6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="236e6-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="236e6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="236e6-123">Authorization</span></span>  | <span data-ttu-id="236e6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="236e6-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="236e6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="236e6-126">Content-Type</span></span>  | <span data-ttu-id="236e6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="236e6-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="236e6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="236e6-128">Request body</span></span>
<span data-ttu-id="236e6-129">В тексте запроса укажите представление объекта [educationAssignmentResource](../resources/educationassignmentresource.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="236e6-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="236e6-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="236e6-130">Response</span></span>
<span data-ttu-id="236e6-131">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [educationAssignmentResource](../resources/educationassignmentresource.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="236e6-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="236e6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="236e6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="236e6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="236e6-133">Request</span></span>
<span data-ttu-id="236e6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="236e6-134">The following is an example of the request.</span></span>
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
<span data-ttu-id="236e6-135">В тексте запроса укажите представление объекта [educationAssignmentResource](../resources/educationassignmentresource.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="236e6-135">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="236e6-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="236e6-136">Response</span></span>
<span data-ttu-id="236e6-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="236e6-137">The following is an example of the response.</span></span> 

><span data-ttu-id="236e6-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="236e6-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="236e6-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="236e6-139">All of the properties will be returned from an actual call.</span></span>


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
<!--
{
  "type": "#page.annotation",
  "description": "Create educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-post-resources.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
