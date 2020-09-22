---
title: Присоединение Едукатионрубрик к educationAssignment
description: Присоединение существующего объекта Едукатионрубрик к educationAssignment.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 765f4e937a60cf4701f9639433794743af6d4dce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007758"
---
# <a name="create-educationrubric"></a><span data-ttu-id="903ec-103">Создание Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="903ec-103">Create educationRubric</span></span>

<span data-ttu-id="903ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="903ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="903ec-105">Присоединение существующего объекта [едукатионрубрик](../resources/educationrubric.md) к [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="903ec-105">Attach an existing [educationRubric](../resources/educationrubric.md) object to an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="903ec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="903ec-106">Permissions</span></span>

<span data-ttu-id="903ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="903ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="903ec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="903ec-109">Permission type</span></span>                        | <span data-ttu-id="903ec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="903ec-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="903ec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="903ec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="903ec-112">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="903ec-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="903ec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="903ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="903ec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="903ec-114">Not supported.</span></span> |
| <span data-ttu-id="903ec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="903ec-115">Application</span></span>                            | <span data-ttu-id="903ec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="903ec-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="903ec-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="903ec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="903ec-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="903ec-118">Request headers</span></span>

| <span data-ttu-id="903ec-119">Имя</span><span class="sxs-lookup"><span data-stu-id="903ec-119">Name</span></span>          | <span data-ttu-id="903ec-120">Описание</span><span class="sxs-lookup"><span data-stu-id="903ec-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="903ec-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="903ec-121">Authorization</span></span> | <span data-ttu-id="903ec-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="903ec-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="903ec-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="903ec-123">Request body</span></span>

<span data-ttu-id="903ec-124">В теле запроса добавьте идентификатор OData существующего объекта [едукатионрубрик](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="903ec-124">In the request body, supply the OData ID of an existing [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="903ec-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="903ec-125">Response</span></span>

<span data-ttu-id="903ec-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="903ec-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="903ec-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="903ec-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="903ec-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="903ec-129">Request</span></span>

<span data-ttu-id="903ec-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="903ec-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="903ec-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="903ec-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_educationassignment"
}-->

```http
PUT https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/rubric/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/education/me/rubrics/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="903ec-132">C#</span><span class="sxs-lookup"><span data-stu-id="903ec-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="903ec-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="903ec-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="903ec-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="903ec-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="903ec-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="903ec-135">Response</span></span>

<span data-ttu-id="903ec-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="903ec-136">The following is an example of the response.</span></span>

> <span data-ttu-id="903ec-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="903ec-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 204 No Content
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


