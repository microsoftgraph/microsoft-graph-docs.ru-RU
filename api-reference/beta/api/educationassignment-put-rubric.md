---
title: Присоединение Едукатионрубрик к educationAssignment
description: Присоединение существующего объекта Едукатионрубрик к educationAssignment.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 84a0f60edfa292776291e823538c45ae7e7d5898
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461157"
---
# <a name="create-educationrubric"></a><span data-ttu-id="81de8-103">Создание Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="81de8-103">Create educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81de8-104">Присоединение существующего объекта [едукатионрубрик](../resources/educationrubric.md) к [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="81de8-104">Attach an existing [educationRubric](../resources/educationrubric.md) object to an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="81de8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="81de8-105">Permissions</span></span>

<span data-ttu-id="81de8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81de8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="81de8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="81de8-108">Permission type</span></span>                        | <span data-ttu-id="81de8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="81de8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="81de8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="81de8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="81de8-111">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="81de8-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="81de8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="81de8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81de8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81de8-113">Not supported.</span></span> |
| <span data-ttu-id="81de8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="81de8-114">Application</span></span>                            | <span data-ttu-id="81de8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81de8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81de8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="81de8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="81de8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="81de8-117">Request headers</span></span>

| <span data-ttu-id="81de8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="81de8-118">Name</span></span>          | <span data-ttu-id="81de8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="81de8-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="81de8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="81de8-120">Authorization</span></span> | <span data-ttu-id="81de8-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="81de8-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="81de8-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="81de8-122">Request body</span></span>

<span data-ttu-id="81de8-123">В теле запроса добавьте идентификатор OData существующего объекта [едукатионрубрик](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="81de8-123">In the request body, supply the OData ID of an existing [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="81de8-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="81de8-124">Response</span></span>

<span data-ttu-id="81de8-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="81de8-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81de8-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="81de8-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81de8-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="81de8-128">Request</span></span>

<span data-ttu-id="81de8-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="81de8-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="81de8-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="81de8-130">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="81de8-131">C#</span><span class="sxs-lookup"><span data-stu-id="81de8-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81de8-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81de8-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="81de8-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="81de8-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="81de8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="81de8-134">Response</span></span>

<span data-ttu-id="81de8-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="81de8-135">The following is an example of the response.</span></span>

> <span data-ttu-id="81de8-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="81de8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
