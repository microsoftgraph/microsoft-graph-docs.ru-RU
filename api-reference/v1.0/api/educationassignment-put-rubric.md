---
title: Присоединение educationRubric к educationAssignment
description: Прикрепить существующий объект educationRubric к educationAssignment.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 51c2cf968f1064b3e8bbe8cb157cb95f8e46d959
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992502"
---
# <a name="attach-educationrubric-to-an-assignment"></a><span data-ttu-id="8d503-103">Присоединение educationRubric к назначению</span><span class="sxs-lookup"><span data-stu-id="8d503-103">Attach educationRubric to an assignment</span></span>

<span data-ttu-id="8d503-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d503-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d503-105">Прикрепить существующий [объект educationRubric](../resources/educationrubric.md) к [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8d503-105">Attach an existing [educationRubric](../resources/educationrubric.md) object to an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8d503-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d503-106">Permissions</span></span>

<span data-ttu-id="8d503-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d503-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d503-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d503-109">Permission type</span></span>                        | <span data-ttu-id="8d503-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d503-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8d503-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d503-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d503-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8d503-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="8d503-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d503-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d503-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d503-114">Not supported.</span></span> |
| <span data-ttu-id="8d503-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d503-115">Application</span></span>                            | <span data-ttu-id="8d503-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d503-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d503-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d503-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="8d503-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d503-118">Request headers</span></span>

| <span data-ttu-id="8d503-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8d503-119">Name</span></span>          | <span data-ttu-id="8d503-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8d503-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8d503-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d503-121">Authorization</span></span> | <span data-ttu-id="8d503-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8d503-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d503-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8d503-123">Request body</span></span>

<span data-ttu-id="8d503-124">В теле запроса укажи ID OData существующего [объекта educationRubric.](../resources/educationrubric.md)</span><span class="sxs-lookup"><span data-stu-id="8d503-124">In the request body, supply the OData ID of an existing [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8d503-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d503-125">Response</span></span>

<span data-ttu-id="8d503-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8d503-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d503-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="8d503-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8d503-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d503-129">Request</span></span>

<span data-ttu-id="8d503-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d503-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8d503-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d503-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["cf6005fc-9e13-44a2-a6ac-a53322006454"],
  "name": "create_educationrubric_from_educationassignment"
}-->

```http
PUT https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/rubric/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d"
}
```
# <a name="c"></a>[<span data-ttu-id="8d503-132">C#</span><span class="sxs-lookup"><span data-stu-id="8d503-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d503-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d503-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d503-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d503-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d503-135">Java</span><span class="sxs-lookup"><span data-stu-id="8d503-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationrubric-from-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8d503-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d503-136">Response</span></span>

<span data-ttu-id="8d503-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8d503-137">The following is an example of the response.</span></span>

> <span data-ttu-id="8d503-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8d503-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 204 No Content

{
}
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


