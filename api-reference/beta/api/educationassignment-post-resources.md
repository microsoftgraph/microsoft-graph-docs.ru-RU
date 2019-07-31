---
title: Создание Едукатионассигнментресаурце
description: OData. Type, указывающая тип создаваемого ресурса. Обратите внимание, что файловые ресурсы сначала необходимо отправить в **ресаурцефолдер**назначений.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 86cf738f7558814a76d07e7a7eb5ffd22d988d29
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955678"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="8e981-104">Создание Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="8e981-104">Create educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e981-105">Создайте [ресурс назначения](../resources/educationassignmentresource.md).</span><span class="sxs-lookup"><span data-stu-id="8e981-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="8e981-106">В самом ресурсе есть @odata. Type, указывающий тип создаваемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="8e981-106">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="8e981-107">Обратите внимание, что файловые ресурсы сначала необходимо отправить в **ресаурцефолдер**назначений.</span><span class="sxs-lookup"><span data-stu-id="8e981-107">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e981-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8e981-108">Permissions</span></span>
<span data-ttu-id="8e981-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e981-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e981-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e981-111">Permission type</span></span>      | <span data-ttu-id="8e981-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e981-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8e981-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e981-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="8e981-114">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8e981-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="8e981-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e981-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8e981-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e981-116">Not supported.</span></span>  |
|<span data-ttu-id="8e981-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8e981-117">Application</span></span> | <span data-ttu-id="8e981-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e981-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="8e981-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e981-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="8e981-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8e981-120">Request headers</span></span>
| <span data-ttu-id="8e981-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e981-121">Header</span></span>       | <span data-ttu-id="8e981-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8e981-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8e981-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8e981-123">Authorization</span></span>  | <span data-ttu-id="8e981-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e981-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8e981-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8e981-126">Content-Type</span></span>  | <span data-ttu-id="8e981-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8e981-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e981-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8e981-128">Request body</span></span>
<span data-ttu-id="8e981-129">В тексте запроса добавьте представление объекта [едукатионассигнментресаурце](../resources/educationassignmentresource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e981-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="8e981-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e981-130">Response</span></span>
<span data-ttu-id="8e981-131">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [едукатионассигнментресаурце](../resources/educationassignmentresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e981-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e981-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8e981-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8e981-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e981-133">Request</span></span>
<span data-ttu-id="8e981-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e981-134">The following is an example of the request.</span></span>
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
<span data-ttu-id="8e981-135">В тексте запроса добавьте представление объекта [едукатионассигнментресаурце](../resources/educationassignmentresource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e981-135">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8e981-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e981-136">Response</span></span>
<span data-ttu-id="8e981-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8e981-137">The following is an example of the response.</span></span> 

><span data-ttu-id="8e981-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8e981-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8e981-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e981-139">All of the properties will be returned from an actual call.</span></span>


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
