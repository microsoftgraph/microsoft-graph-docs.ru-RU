---
title: Создание Едукатионассигнментресаурце
description: OData. Type, указывающая тип создаваемого ресурса. Обратите внимание, что файловые ресурсы сначала необходимо отправить в **ресаурцефолдер**назначений.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 408ff1b44fda0d4e9b6f16c2234ed06a4ca24852
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324723"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="48e2d-104">Создание Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="48e2d-104">Create educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48e2d-105">Создайте [ресурс назначения](../resources/educationassignmentresource.md).</span><span class="sxs-lookup"><span data-stu-id="48e2d-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="48e2d-106">В самом ресурсе есть @odata. Type, указывающий тип создаваемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="48e2d-106">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="48e2d-107">Обратите внимание, что файловые ресурсы сначала необходимо отправить в **ресаурцефолдер**назначений.</span><span class="sxs-lookup"><span data-stu-id="48e2d-107">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="48e2d-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48e2d-108">Permissions</span></span>
<span data-ttu-id="48e2d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48e2d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48e2d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48e2d-111">Permission type</span></span>      | <span data-ttu-id="48e2d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48e2d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48e2d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48e2d-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="48e2d-114">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="48e2d-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="48e2d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48e2d-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="48e2d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48e2d-116">Not supported.</span></span>  |
|<span data-ttu-id="48e2d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48e2d-117">Application</span></span> | <span data-ttu-id="48e2d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48e2d-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="48e2d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48e2d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="48e2d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48e2d-120">Request headers</span></span>
| <span data-ttu-id="48e2d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="48e2d-121">Header</span></span>       | <span data-ttu-id="48e2d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="48e2d-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="48e2d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48e2d-123">Authorization</span></span>  | <span data-ttu-id="48e2d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="48e2d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="48e2d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48e2d-126">Content-Type</span></span>  | <span data-ttu-id="48e2d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="48e2d-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="48e2d-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48e2d-128">Request body</span></span>
<span data-ttu-id="48e2d-129">В тексте запроса добавьте представление объекта [едукатионассигнментресаурце](../resources/educationassignmentresource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48e2d-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="48e2d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="48e2d-130">Response</span></span>
<span data-ttu-id="48e2d-131">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [едукатионассигнментресаурце](../resources/educationassignmentresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48e2d-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48e2d-132">Пример</span><span class="sxs-lookup"><span data-stu-id="48e2d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48e2d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="48e2d-133">Request</span></span>
<span data-ttu-id="48e2d-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48e2d-134">The following is an example of the request.</span></span>
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
<span data-ttu-id="48e2d-135">В тексте запроса добавьте представление объекта [едукатионассигнментресаурце](../resources/educationassignmentresource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48e2d-135">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="48e2d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="48e2d-136">Response</span></span>
<span data-ttu-id="48e2d-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="48e2d-137">The following is an example of the response.</span></span> 

><span data-ttu-id="48e2d-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="48e2d-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="48e2d-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48e2d-139">All of the properties will be returned from an actual call.</span></span>


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
  "suppressions": []
}
-->
