---
title: Создание educationAssignmentResource
description: Создание ресурса назначения образования.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3ca73c7b078520f5f25b0948b8a41f272ba73669
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911895"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="36383-103">Создание educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="36383-103">Create educationAssignmentResource</span></span>

<span data-ttu-id="36383-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36383-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36383-105">Создание ресурса [назначения.](../resources/educationassignmentresource.md)</span><span class="sxs-lookup"><span data-stu-id="36383-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> <span data-ttu-id="36383-106">Сам ресурс имеет @odata.type, чтобы указать тип создаемого ресурса.</span><span class="sxs-lookup"><span data-stu-id="36383-106">The resource itself has an @odata.type to indicate which type of resource is being created.</span></span> <span data-ttu-id="36383-107">Обратите внимание, что сначала ресурсы на основе файлов должны быть загружены в ресурс **назначенийFolder.**</span><span class="sxs-lookup"><span data-stu-id="36383-107">Note that file-based resources must first be uploaded to the assignments **resourceFolder**.</span></span>

## <a name="permissions"></a><span data-ttu-id="36383-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36383-108">Permissions</span></span>
<span data-ttu-id="36383-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36383-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36383-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36383-111">Permission type</span></span>      | <span data-ttu-id="36383-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36383-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36383-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36383-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="36383-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36383-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="36383-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36383-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="36383-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36383-116">Not supported.</span></span>  |
|<span data-ttu-id="36383-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36383-117">Application</span></span> | <span data-ttu-id="36383-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36383-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="36383-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36383-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="36383-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36383-120">Request headers</span></span>
| <span data-ttu-id="36383-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36383-121">Header</span></span>       | <span data-ttu-id="36383-122">Значение</span><span class="sxs-lookup"><span data-stu-id="36383-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="36383-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36383-123">Authorization</span></span>  | <span data-ttu-id="36383-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36383-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="36383-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="36383-126">Content-Type</span></span>  | <span data-ttu-id="36383-127">application/json</span><span class="sxs-lookup"><span data-stu-id="36383-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36383-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="36383-128">Request body</span></span>
<span data-ttu-id="36383-129">В теле запроса поставляют представление JSON объекта [educationAssignmentResource.](../resources/educationassignmentresource.md)</span><span class="sxs-lookup"><span data-stu-id="36383-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="36383-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="36383-130">Response</span></span>
<span data-ttu-id="36383-131">В случае успешного выполнения этот метод возвращает код ответа и `201 Created` объект [educationAssignmentResource](../resources/educationassignmentresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="36383-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36383-132">Пример</span><span class="sxs-lookup"><span data-stu-id="36383-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36383-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="36383-133">Request</span></span>
<span data-ttu-id="36383-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36383-134">The following is an example of the request.</span></span>
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
<span data-ttu-id="36383-135">В теле запроса поставляют представление JSON объекта [educationAssignmentResource.](../resources/educationassignmentresource.md)</span><span class="sxs-lookup"><span data-stu-id="36383-135">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="36383-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="36383-136">Response</span></span>
<span data-ttu-id="36383-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="36383-137">The following is an example of the response.</span></span> 

><span data-ttu-id="36383-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="36383-138">**Note:** The response object shown here might be shortened for readability.</span></span>


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


