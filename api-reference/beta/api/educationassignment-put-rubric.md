---
title: Присоединение Едукатионрубрик к educationAssignment
description: Присоединение существующего объекта Едукатионрубрик к educationAssignment.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 913ab8805b7ef5b14fb58d9d3bf01553efff8cc5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427349"
---
# <a name="create-educationrubric"></a><span data-ttu-id="72a9e-103">Создание Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="72a9e-103">Create educationRubric</span></span>

<span data-ttu-id="72a9e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="72a9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72a9e-105">Присоединение существующего объекта [едукатионрубрик](../resources/educationrubric.md) к [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="72a9e-105">Attach an existing [educationRubric](../resources/educationrubric.md) object to an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="72a9e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72a9e-106">Permissions</span></span>

<span data-ttu-id="72a9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72a9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72a9e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72a9e-109">Permission type</span></span>                        | <span data-ttu-id="72a9e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72a9e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="72a9e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72a9e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="72a9e-112">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72a9e-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="72a9e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72a9e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72a9e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72a9e-114">Not supported.</span></span> |
| <span data-ttu-id="72a9e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72a9e-115">Application</span></span>                            | <span data-ttu-id="72a9e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72a9e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72a9e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72a9e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="72a9e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72a9e-118">Request headers</span></span>

| <span data-ttu-id="72a9e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="72a9e-119">Name</span></span>          | <span data-ttu-id="72a9e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="72a9e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="72a9e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="72a9e-121">Authorization</span></span> | <span data-ttu-id="72a9e-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="72a9e-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="72a9e-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="72a9e-123">Request body</span></span>

<span data-ttu-id="72a9e-124">В теле запроса добавьте идентификатор OData существующего объекта [едукатионрубрик](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="72a9e-124">In the request body, supply the OData ID of an existing [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="72a9e-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="72a9e-125">Response</span></span>

<span data-ttu-id="72a9e-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="72a9e-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72a9e-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="72a9e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72a9e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="72a9e-129">Request</span></span>

<span data-ttu-id="72a9e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72a9e-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72a9e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="72a9e-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="72a9e-132">C#</span><span class="sxs-lookup"><span data-stu-id="72a9e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72a9e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72a9e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72a9e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72a9e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="72a9e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="72a9e-135">Response</span></span>

<span data-ttu-id="72a9e-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="72a9e-136">The following is an example of the response.</span></span>

> <span data-ttu-id="72a9e-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72a9e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
