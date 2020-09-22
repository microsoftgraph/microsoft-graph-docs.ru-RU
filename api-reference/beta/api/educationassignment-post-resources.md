---
title: Создание Едукатионассигнментресаурце
description: OData. Type, указывающая тип создаваемого ресурса. Обратите внимание, что файловые ресурсы сначала необходимо отправить в **ресаурцефолдер**назначений.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1e432d4521ffe871de75be4ae8764953d99a3abc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002557"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="68af5-104">Создание Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="68af5-104">Create educationAssignmentResource</span></span>

<span data-ttu-id="68af5-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68af5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68af5-106">Создайте [ресурс назначения](../resources/educationassignmentresource.md).</span><span class="sxs-lookup"><span data-stu-id="68af5-106">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="68af5-107">В самом ресурсе есть @odata. Type, указывающий тип создаваемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="68af5-107">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="68af5-108">Обратите внимание, что файловые ресурсы сначала необходимо отправить в **ресаурцефолдер**назначений.</span><span class="sxs-lookup"><span data-stu-id="68af5-108">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="68af5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68af5-109">Permissions</span></span>
<span data-ttu-id="68af5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68af5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68af5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68af5-112">Permission type</span></span>      | <span data-ttu-id="68af5-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68af5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68af5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68af5-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="68af5-115">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68af5-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="68af5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68af5-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="68af5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68af5-117">Not supported.</span></span>  |
|<span data-ttu-id="68af5-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68af5-118">Application</span></span> | <span data-ttu-id="68af5-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68af5-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="68af5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68af5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="68af5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68af5-121">Request headers</span></span>
| <span data-ttu-id="68af5-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68af5-122">Header</span></span>       | <span data-ttu-id="68af5-123">Значение</span><span class="sxs-lookup"><span data-stu-id="68af5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="68af5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68af5-124">Authorization</span></span>  | <span data-ttu-id="68af5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68af5-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="68af5-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68af5-127">Content-Type</span></span>  | <span data-ttu-id="68af5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="68af5-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="68af5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68af5-129">Request body</span></span>
<span data-ttu-id="68af5-130">В тексте запроса добавьте представление объекта [едукатионассигнментресаурце](../resources/educationassignmentresource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68af5-130">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="68af5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="68af5-131">Response</span></span>
<span data-ttu-id="68af5-132">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [едукатионассигнментресаурце](../resources/educationassignmentresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68af5-132">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68af5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="68af5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68af5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="68af5-134">Request</span></span>
<span data-ttu-id="68af5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68af5-135">The following is an example of the request.</span></span>
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
<span data-ttu-id="68af5-136">В тексте запроса добавьте представление объекта [едукатионассигнментресаурце](../resources/educationassignmentresource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68af5-136">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="68af5-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="68af5-137">Response</span></span>
<span data-ttu-id="68af5-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="68af5-138">The following is an example of the response.</span></span> 

><span data-ttu-id="68af5-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="68af5-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="68af5-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68af5-140">All of the properties will be returned from an actual call.</span></span>


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


